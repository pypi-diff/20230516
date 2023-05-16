# Comparing `tmp/syscryptaddition-1.0.0.tar.gz` & `tmp/syscryptaddition-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscryptaddition-1.0.0.tar", last modified: Tue May 16 20:22:35 2023, max compression
+gzip compressed data, was "syscryptaddition-1.1.0.tar", last modified: Tue May 16 20:24:41 2023, max compression
```

## Comparing `syscryptaddition-1.0.0.tar` & `syscryptaddition-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:22:35.546328 syscryptaddition-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-16 20:22:35.546328 syscryptaddition-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 20:22:35.546328 syscryptaddition-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      562 2023-05-16 20:22:35.000000 syscryptaddition-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:22:35.546328 syscryptaddition-1.0.0/syscryptaddition/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 20:22:35.000000 syscryptaddition-1.0.0/syscryptaddition/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:22:35.546328 syscryptaddition-1.0.0/syscryptaddition.egg-info/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-16 20:22:35.000000 syscryptaddition-1.0.0/syscryptaddition.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-16 20:22:35.000000 syscryptaddition-1.0.0/syscryptaddition.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 20:22:35.000000 syscryptaddition-1.0.0/syscryptaddition.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-16 20:22:35.000000 syscryptaddition-1.0.0/syscryptaddition.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:24:41.033062 syscryptaddition-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-16 20:24:41.033062 syscryptaddition-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 20:24:41.033062 syscryptaddition-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      562 2023-05-16 20:24:40.000000 syscryptaddition-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:24:41.033062 syscryptaddition-1.1.0/syscryptaddition/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-16 20:24:40.000000 syscryptaddition-1.1.0/syscryptaddition/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:24:41.033062 syscryptaddition-1.1.0/syscryptaddition.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-16 20:24:40.000000 syscryptaddition-1.1.0/syscryptaddition.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-16 20:24:41.000000 syscryptaddition-1.1.0/syscryptaddition.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 20:24:40.000000 syscryptaddition-1.1.0/syscryptaddition.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-16 20:24:40.000000 syscryptaddition-1.1.0/syscryptaddition.egg-info/top_level.txt
```

### Comparing `syscryptaddition-1.0.0/setup.py` & `syscryptaddition-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syscryptaddition",
     version=VERSION,
```

