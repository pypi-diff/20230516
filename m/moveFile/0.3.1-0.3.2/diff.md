# Comparing `tmp/MoveFile-0.3.1.tar.gz` & `tmp/MoveFile-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MoveFile-0.3.1.tar", last modified: Thu May 11 09:52:23 2023, max compression
+gzip compressed data, was "MoveFile-0.3.2.tar", last modified: Tue May 16 05:44:59 2023, max compression
```

## Comparing `MoveFile-0.3.1.tar` & `MoveFile-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 09:52:23.311608 MoveFile-0.3.1/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 MoveFile-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 MoveFile-0.3.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-11 09:52:23.294606 MoveFile-0.3.1/MoveFile.egg-info/
--rw-rw-rw-   0        0        0      409 2023-05-11 09:52:23.000000 MoveFile-0.3.1/MoveFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-05-11 09:52:23.000000 MoveFile-0.3.1/MoveFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 09:52:23.000000 MoveFile-0.3.1/MoveFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-11 09:52:23.000000 MoveFile-0.3.1/MoveFile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      409 2023-05-11 09:52:23.311608 MoveFile-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-22 07:19:14.000000 MoveFile-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 09:52:23.305603 MoveFile-0.3.1/moveFile/
-drwxrwxrwx   0        0        0        0 2023-05-11 09:52:23.309604 MoveFile-0.3.1/moveFile/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 MoveFile-0.3.1/moveFile/Ui/__init__.py
--rw-rw-rw-   0        0        0    71168 2023-04-28 06:15:40.000000 MoveFile-0.3.1/moveFile/Ui/moveFileUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 MoveFile-0.3.1/moveFile/__init__.py
--rw-rw-rw-   0        0        0    35840 2023-04-28 06:14:13.000000 MoveFile-0.3.1/moveFile/find_file_return_path_m1.pyd
--rw-rw-rw-   0        0        0   228352 2023-05-11 09:48:11.000000 MoveFile-0.3.1/moveFile/moveFile.pyd
--rw-rw-rw-   0        0        0    68608 2023-04-28 06:14:21.000000 MoveFile-0.3.1/moveFile/moveFileUi.pyd
--rw-rw-rw-   0        0        0    69632 2023-04-28 06:14:45.000000 MoveFile-0.3.1/moveFile/optionDb.pyd
--rw-rw-rw-   0        0        0      135 2023-05-11 09:52:23.312605 MoveFile-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1054 2023-05-11 09:51:12.000000 MoveFile-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:44:59.744875 MoveFile-0.3.2/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 MoveFile-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 MoveFile-0.3.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-16 05:44:59.726024 MoveFile-0.3.2/MoveFile.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-05-16 05:44:59.000000 MoveFile-0.3.2/MoveFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-05-16 05:44:59.000000 MoveFile-0.3.2/MoveFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 05:44:59.000000 MoveFile-0.3.2/MoveFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 05:44:59.000000 MoveFile-0.3.2/MoveFile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      409 2023-05-16 05:44:59.745876 MoveFile-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-22 07:19:14.000000 MoveFile-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 05:44:59.737875 MoveFile-0.3.2/moveFile/
+drwxrwxrwx   0        0        0        0 2023-05-16 05:44:59.742875 MoveFile-0.3.2/moveFile/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 MoveFile-0.3.2/moveFile/Ui/__init__.py
+-rw-rw-rw-   0        0        0    71168 2023-04-28 06:15:40.000000 MoveFile-0.3.2/moveFile/Ui/moveFileUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 MoveFile-0.3.2/moveFile/__init__.py
+-rw-rw-rw-   0        0        0    35840 2023-04-28 06:14:13.000000 MoveFile-0.3.2/moveFile/find_file_return_path_m1.pyd
+-rw-rw-rw-   0        0        0   228352 2023-05-16 05:44:06.000000 MoveFile-0.3.2/moveFile/moveFile.pyd
+-rw-rw-rw-   0        0        0    68608 2023-04-28 06:14:21.000000 MoveFile-0.3.2/moveFile/moveFileUi.pyd
+-rw-rw-rw-   0        0        0    69632 2023-04-28 06:14:45.000000 MoveFile-0.3.2/moveFile/optionDb.pyd
+-rw-rw-rw-   0        0        0      135 2023-05-16 05:44:59.746876 MoveFile-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2023-05-16 05:42:01.000000 MoveFile-0.3.2/setup.py
```

### Comparing `MoveFile-0.3.1/LICENSE.txt` & `MoveFile-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MoveFile-0.3.1/setup.py` & `MoveFile-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 1
+PATCH = 2
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "MoveFile",
```

