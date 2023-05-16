# Comparing `tmp/ApReusable-1.3.1.tar.gz` & `tmp/ApReusable-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ApReusable-1.3.1.tar", last modified: Tue May 16 06:03:07 2023, max compression
+gzip compressed data, was "ApReusable-1.3.2.tar", last modified: Tue May 16 06:05:33 2023, max compression
```

## Comparing `ApReusable-1.3.1.tar` & `ApReusable-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:07.528355 ApReusable-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:07.524355 ApReusable-1.3.1/ApReusable/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 06:02:56.000000 ApReusable-1.3.1/ApReusable/ExtendedEnum.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:02:56.000000 ApReusable-1.3.1/ApReusable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-16 06:02:56.000000 ApReusable-1.3.1/ApReusable/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:02:56.000000 ApReusable-1.3.1/ApReusable/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-16 06:02:56.000000 ApReusable-1.3.1/ApReusable/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 06:02:56.000000 ApReusable-1.3.1/ApReusable/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:07.528355 ApReusable-1.3.1/ApReusable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-16 06:03:07.000000 ApReusable-1.3.1/ApReusable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-16 06:03:07.000000 ApReusable-1.3.1/ApReusable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:03:07.000000 ApReusable-1.3.1/ApReusable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 06:03:07.000000 ApReusable-1.3.1/ApReusable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 06:03:07.000000 ApReusable-1.3.1/ApReusable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-16 06:03:07.528355 ApReusable-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-16 06:02:56.000000 ApReusable-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:03:07.528355 ApReusable-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-16 06:02:56.000000 ApReusable-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:05:33.383376 ApReusable-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:05:33.383376 ApReusable-1.3.2/ApReusable/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 06:05:22.000000 ApReusable-1.3.2/ApReusable/ExtendedEnum.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:05:22.000000 ApReusable-1.3.2/ApReusable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-16 06:05:22.000000 ApReusable-1.3.2/ApReusable/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:05:22.000000 ApReusable-1.3.2/ApReusable/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-16 06:05:22.000000 ApReusable-1.3.2/ApReusable/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 06:05:22.000000 ApReusable-1.3.2/ApReusable/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:05:33.383376 ApReusable-1.3.2/ApReusable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-16 06:05:33.000000 ApReusable-1.3.2/ApReusable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-16 06:05:33.000000 ApReusable-1.3.2/ApReusable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:05:33.000000 ApReusable-1.3.2/ApReusable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 06:05:33.000000 ApReusable-1.3.2/ApReusable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 06:05:33.000000 ApReusable-1.3.2/ApReusable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-16 06:05:33.383376 ApReusable-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-16 06:05:22.000000 ApReusable-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:05:33.383376 ApReusable-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-16 06:05:22.000000 ApReusable-1.3.2/setup.py
```

### Comparing `ApReusable-1.3.1/ApReusable/functions.py` & `ApReusable-1.3.2/ApReusable/functions.py`

 * *Files identical despite different names*

### Comparing `ApReusable-1.3.1/ApReusable/renderer.py` & `ApReusable-1.3.2/ApReusable/renderer.py`

 * *Files identical despite different names*

### Comparing `ApReusable-1.3.1/ApReusable.egg-info/PKG-INFO` & `ApReusable-1.3.2/ApReusable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApReusable
-Version: 1.3.1
+Version: 1.3.2
 Summary: AP-Reusable-Package is a versatile and powerful Python package that contains many useful functions and classes for a wide range of projects.
 Author: Rafat & Billah
 Author-email: support@aamarpay.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `ApReusable-1.3.1/PKG-INFO` & `ApReusable-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApReusable
-Version: 1.3.1
+Version: 1.3.2
 Summary: AP-Reusable-Package is a versatile and powerful Python package that contains many useful functions and classes for a wide range of projects.
 Author: Rafat & Billah
 Author-email: support@aamarpay.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `ApReusable-1.3.1/README.md` & `ApReusable-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ApReusable-1.3.1/setup.py` & `ApReusable-1.3.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'cryptography>=39.0',
     'Django>=4.0',
     'djangorestframework>=3.0'
 ]
 
 setuptools.setup(
     name='ApReusable',
-    version='1.3.1',
+    version='1.3.2',
     description='AP-Reusable-Package is a versatile and powerful Python package that contains many useful functions and classes for a wide range of projects.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Rafat & Billah',
     author_email='support@aamarpay.com',
     license='MIT',
     classifiers=classifiers,
```

