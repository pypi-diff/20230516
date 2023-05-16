# Comparing `tmp/syscolouraddons-1.0.0.tar.gz` & `tmp/syscolouraddons-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscolouraddons-1.0.0.tar", last modified: Tue May 16 04:20:49 2023, max compression
+gzip compressed data, was "syscolouraddons-1.1.0.tar", last modified: Tue May 16 04:22:56 2023, max compression
```

## Comparing `syscolouraddons-1.0.0.tar` & `syscolouraddons-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:20:49.411714 syscolouraddons-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-16 04:20:49.411714 syscolouraddons-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 04:20:49.411714 syscolouraddons-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      561 2023-05-16 04:20:49.000000 syscolouraddons-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:20:49.411714 syscolouraddons-1.0.0/syscolouraddons/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 04:20:49.000000 syscolouraddons-1.0.0/syscolouraddons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:20:49.411714 syscolouraddons-1.0.0/syscolouraddons.egg-info/
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-16 04:20:49.000000 syscolouraddons-1.0.0/syscolouraddons.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-16 04:20:49.000000 syscolouraddons-1.0.0/syscolouraddons.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 04:20:49.000000 syscolouraddons-1.0.0/syscolouraddons.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-16 04:20:49.000000 syscolouraddons-1.0.0/syscolouraddons.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:22:56.270162 syscolouraddons-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-16 04:22:56.270162 syscolouraddons-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 04:22:56.270162 syscolouraddons-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      561 2023-05-16 04:22:56.000000 syscolouraddons-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:22:56.270162 syscolouraddons-1.1.0/syscolouraddons/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-16 04:22:56.000000 syscolouraddons-1.1.0/syscolouraddons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 04:22:56.270162 syscolouraddons-1.1.0/syscolouraddons.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-16 04:22:56.000000 syscolouraddons-1.1.0/syscolouraddons.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-16 04:22:56.000000 syscolouraddons-1.1.0/syscolouraddons.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 04:22:56.000000 syscolouraddons-1.1.0/syscolouraddons.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-16 04:22:56.000000 syscolouraddons-1.1.0/syscolouraddons.egg-info/top_level.txt
```

### Comparing `syscolouraddons-1.0.0/setup.py` & `syscolouraddons-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syscolouraddons",
     version=VERSION,
```

