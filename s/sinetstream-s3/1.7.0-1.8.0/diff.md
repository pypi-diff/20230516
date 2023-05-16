# Comparing `tmp/sinetstream-s3-1.7.0.tar.gz` & `tmp/sinetstream-s3-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream-s3-1.7.0.tar", last modified: Fri Sep 16 07:09:26 2022, max compression
+gzip compressed data, was "sinetstream-s3-1.8.0.tar", last modified: Tue May 16 06:40:43 2023, max compression
```

## Comparing `sinetstream-s3-1.7.0.tar` & `sinetstream-s3-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:26.881434 sinetstream-s3-1.7.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)      580 2022-09-16 07:09:26.881434 sinetstream-s3-1.7.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)     1605 2022-09-16 07:09:26.881434 sinetstream-s3-1.7.0/setup.cfg
--rw-rw-r--   0 koie      (1004) koie      (1004)       39 2022-09-15 07:30:59.000000 sinetstream-s3-1.7.0/setup.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:26.877434 sinetstream-s3-1.7.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:26.881434 sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)      580 2022-09-16 07:09:26.000000 sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      392 2022-09-16 07:09:26.000000 sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2022-09-16 07:09:26.000000 sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)      250 2022-09-16 07:09:26.000000 sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/entry_points.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2022-09-16 07:09:26.000000 sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/namespace_packages.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2022-09-16 07:07:30.000000 sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)       25 2022-09-16 07:09:26.000000 sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2022-09-16 07:09:26.000000 sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/top_level.txt
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:26.881434 sinetstream-s3-1.7.0/src/sinetstreamplugin/
--rw-rw-r--   0 koie      (1004) koie      (1004)    14948 2022-09-15 07:30:59.000000 sinetstream-s3-1.7.0/src/sinetstreamplugin/s3.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      541 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1612 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/setup.cfg
+-rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-01-12 00:12:25.000000 sinetstream-s3-1.8.0/setup.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:43.222475 sinetstream-s3-1.8.0/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      541 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      392 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)      249 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/entry_points.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/namespace_packages.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-01-12 00:15:59.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)       25 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:40:43.000000 sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:43.230475 sinetstream-s3-1.8.0/src/sinetstreamplugin/
+-rw-rw-r--   0 koie      (1004) koie      (1004)    14948 2023-01-12 00:12:25.000000 sinetstream-s3-1.8.0/src/sinetstreamplugin/s3.py
```

### Comparing `sinetstream-s3-1.7.0/PKG-INFO` & `sinetstream-s3-1.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sinetstream-s3
-Version: 1.7.0
+Version: 1.8.0
 Summary: S3 plugin for SINETStream library
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

### Comparing `sinetstream-s3-1.7.0/setup.cfg` & `sinetstream-s3-1.8.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinetstream-s3
-version = 1.7.0
+version = 1.8.0
 description = S3 plugin for SINETStream library
 license = Apache License, Version 2.0
 license_files = 
 	../../../../LICENSE
 url = https://github.com/nii-gakunin-cloud/sinetstream
 classifiers = 
 	Development Status :: 4 - Beta
@@ -16,22 +16,22 @@
 
 [options]
 package_dir = 
 	=src
 packages = find_namespace:
 zip_safe = False
 install_requires = 
-	sinetstream>=1.7.0
+	sinetstream>=1.8.0
 	boto3
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

### Comparing `sinetstream-s3-1.7.0/src/sinetstream_s3.egg-info/PKG-INFO` & `sinetstream-s3-1.8.0/src/sinetstream_s3.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sinetstream-s3
-Version: 1.7.0
+Version: 1.8.0
 Summary: S3 plugin for SINETStream library
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

### Comparing `sinetstream-s3-1.7.0/src/sinetstreamplugin/s3.py` & `sinetstream-s3-1.8.0/src/sinetstreamplugin/s3.py`

 * *Files identical despite different names*

