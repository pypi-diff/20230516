# Comparing `tmp/makeWordQrpics-0.3.1.tar.gz` & `tmp/makeWordQrpics-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makeWordQrpics-0.3.1.tar", last modified: Fri May  5 12:41:16 2023, max compression
+gzip compressed data, was "makeWordQrpics-0.3.2.tar", last modified: Tue May 16 03:47:06 2023, max compression
```

## Comparing `makeWordQrpics-0.3.1.tar` & `makeWordQrpics-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.622435 makeWordQrpics-0.3.1/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 makeWordQrpics-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 makeWordQrpics-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      424 2023-05-05 12:41:16.622435 makeWordQrpics-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 makeWordQrpics-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.606354 makeWordQrpics-0.3.1/makeWordQrpics/
-drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.615436 makeWordQrpics-0.3.1/makeWordQrpics/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 06:42:06.000000 makeWordQrpics-0.3.1/makeWordQrpics/Function/__init__.py
--rw-rw-rw-   0        0        0     5573 2022-11-23 09:35:24.000000 makeWordQrpics-0.3.1/makeWordQrpics/Function/optionDb.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.620463 makeWordQrpics-0.3.1/makeWordQrpics/Ui/
--rw-rw-rw-   0        0        0     5422 2023-02-28 06:51:36.000000 makeWordQrpics-0.3.1/makeWordQrpics/Ui/TableToWordUi.py
--rw-rw-rw-   0        0        0        0 2023-02-28 06:41:59.000000 makeWordQrpics-0.3.1/makeWordQrpics/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 06:54:16.000000 makeWordQrpics-0.3.1/makeWordQrpics/__init__.py
--rw-rw-rw-   0        0        0    11319 2023-02-28 06:59:23.000000 makeWordQrpics-0.3.1/makeWordQrpics/make_word_qrpics.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:41:16.612438 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/
--rw-rw-rw-   0        0        0      424 2023-05-05 12:41:16.000000 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-05-05 12:41:16.000000 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:41:16.000000 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-05 12:41:16.000000 makeWordQrpics-0.3.1/makeWordQrpics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2023-05-05 12:41:16.623436 makeWordQrpics-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      970 2023-05-05 12:41:04.000000 makeWordQrpics-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:47:06.626703 makeWordQrpics-0.3.2/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 makeWordQrpics-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 makeWordQrpics-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      415 2023-05-16 03:47:06.626703 makeWordQrpics-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 makeWordQrpics-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 03:47:06.605708 makeWordQrpics-0.3.2/makeWordQrpics/
+drwxrwxrwx   0        0        0        0 2023-05-16 03:47:06.617710 makeWordQrpics-0.3.2/makeWordQrpics/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 07:01:00.000000 makeWordQrpics-0.3.2/makeWordQrpics/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-04-28 05:55:50.000000 makeWordQrpics-0.3.2/makeWordQrpics/Function/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-05-16 03:47:06.624704 makeWordQrpics-0.3.2/makeWordQrpics/Ui/
+-rw-rw-rw-   0        0        0    72704 2023-04-28 05:55:58.000000 makeWordQrpics-0.3.2/makeWordQrpics/Ui/TableToWordUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 07:01:00.000000 makeWordQrpics-0.3.2/makeWordQrpics/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 07:01:00.000000 makeWordQrpics-0.3.2/makeWordQrpics/__init__.py
+-rw-rw-rw-   0        0        0   142848 2023-05-12 01:18:57.000000 makeWordQrpics-0.3.2/makeWordQrpics/makeWordQrpics.pyd
+drwxrwxrwx   0        0        0        0 2023-05-16 03:47:06.613707 makeWordQrpics-0.3.2/makeWordQrpics.egg-info/
+-rw-rw-rw-   0        0        0      415 2023-05-16 03:47:06.000000 makeWordQrpics-0.3.2/makeWordQrpics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-05-16 03:47:06.000000 makeWordQrpics-0.3.2/makeWordQrpics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 03:47:06.000000 makeWordQrpics-0.3.2/makeWordQrpics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-16 03:47:06.000000 makeWordQrpics-0.3.2/makeWordQrpics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      135 2023-05-16 03:47:06.627703 makeWordQrpics-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-05-16 03:45:59.000000 makeWordQrpics-0.3.2/setup.py
```

### Comparing `makeWordQrpics-0.3.1/LICENSE.txt` & `makeWordQrpics-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `makeWordQrpics-0.3.1/setup.py` & `makeWordQrpics-0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH =1
+PATCH = 2
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "makeWordQrpics",
 	version = VERSION,
     author ="wangweidong",
     author_email = "17891967090@163.com",
-    description='PDF撕裂者单个功能',
+    description='Due Diligence Toolkit Python project',
     long_description_content_type="text/markdown",
 	url = 'https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
 	long_description = open('README.md',encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
 
 	packages = find_packages(),
```

