# Comparing `tmp/pyelib-0.0.2.tar.gz` & `tmp/pyelib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelib-0.0.2.tar", last modified: Tue May 16 10:58:37 2023, max compression
+gzip compressed data, was "pyelib-0.0.3.tar", last modified: Tue May 16 13:56:49 2023, max compression
```

## Comparing `pyelib-0.0.2.tar` & `pyelib-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:37.942125 pyelib-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 10:58:35.000000 pyelib-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-16 10:58:37.942125 pyelib-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-16 10:58:35.000000 pyelib-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:37.942125 pyelib-0.0.2/elib/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 10:58:35.000000 pyelib-0.0.2/elib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-16 10:58:35.000000 pyelib-0.0.2/elib/mongdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:37.942125 pyelib-0.0.2/pyelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-16 10:58:37.000000 pyelib-0.0.2/pyelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-16 10:58:37.000000 pyelib-0.0.2/pyelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:58:37.000000 pyelib-0.0.2/pyelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 10:58:37.000000 pyelib-0.0.2/pyelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 10:58:37.000000 pyelib-0.0.2/pyelib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:58:37.942125 pyelib-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-16 10:58:37.000000 pyelib-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:56:49.611465 pyelib-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 13:56:44.000000 pyelib-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-16 13:56:49.611465 pyelib-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-16 13:56:44.000000 pyelib-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:56:49.611465 pyelib-0.0.3/elib/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 13:56:44.000000 pyelib-0.0.3/elib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-16 13:56:44.000000 pyelib-0.0.3/elib/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-16 13:56:44.000000 pyelib-0.0.3/elib/mongdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:56:49.611465 pyelib-0.0.3/pyelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-16 13:56:49.000000 pyelib-0.0.3/pyelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-16 13:56:49.000000 pyelib-0.0.3/pyelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:56:49.000000 pyelib-0.0.3/pyelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:56:49.000000 pyelib-0.0.3/pyelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 13:56:49.000000 pyelib-0.0.3/pyelib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:56:49.611465 pyelib-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-16 13:56:47.000000 pyelib-0.0.3/setup.py
```

### Comparing `pyelib-0.0.2/LICENSE` & `pyelib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyelib-0.0.2/PKG-INFO` & `pyelib-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyelib
-Version: 0.0.2
+Version: 0.0.3
 Summary: pyelib是一个Python库，为标准库和第三方库提供易于使用的函数封装。
 Home-page: https://github.com/xuehangcang/pyelib
 Author: Xuehang Cang
 Author-email: xuehangcang@outlook.com
 Keywords: pymongo
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `pyelib-0.0.2/README.md` & `pyelib-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyelib-0.0.2/elib/mongdb.py` & `pyelib-0.0.3/elib/mongdb.py`

 * *Files identical despite different names*

### Comparing `pyelib-0.0.2/pyelib.egg-info/PKG-INFO` & `pyelib-0.0.3/pyelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyelib
-Version: 0.0.2
+Version: 0.0.3
 Summary: pyelib是一个Python库，为标准库和第三方库提供易于使用的函数封装。
 Home-page: https://github.com/xuehangcang/pyelib
 Author: Xuehang Cang
 Author-email: xuehangcang@outlook.com
 Keywords: pymongo
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `pyelib-0.0.2/setup.py` & `pyelib-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 PACKAGE_NAME = "pyelib"
 DESCRIPTION = 'pyelib是一个Python库，为标准库和第三方库提供易于使用的函数封装。'
 LONG_DESCRIPTION = 'pyelib是一个Python库，为标准库和第三方库提供易于使用的函数封装。'
 AUTHOR_NAME = "Xuehang Cang"
 AUTHOR_EMAIL = "xuehangcang@outlook.com"
 PROJECT_URL = "https://github.com/xuehangcang/pyelib"
```

