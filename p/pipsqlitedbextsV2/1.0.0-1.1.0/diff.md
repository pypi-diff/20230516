# Comparing `tmp/pipsqlitedbextsV2-1.0.0.tar.gz` & `tmp/pipsqlitedbextsV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlitedbextsV2-1.0.0.tar", last modified: Tue May 16 20:10:05 2023, max compression
+gzip compressed data, was "pipsqlitedbextsV2-1.1.0.tar", last modified: Tue May 16 20:12:11 2023, max compression
```

## Comparing `pipsqlitedbextsV2-1.0.0.tar` & `pipsqlitedbextsV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:10:05.571380 pipsqlitedbextsV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-16 20:10:05.571380 pipsqlitedbextsV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:10:05.571380 pipsqlitedbextsV2-1.0.0/pipsqlitedbextsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 20:10:05.000000 pipsqlitedbextsV2-1.0.0/pipsqlitedbextsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:10:05.571380 pipsqlitedbextsV2-1.0.0/pipsqlitedbextsV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-16 20:10:05.000000 pipsqlitedbextsV2-1.0.0/pipsqlitedbextsV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-16 20:10:05.000000 pipsqlitedbextsV2-1.0.0/pipsqlitedbextsV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 20:10:05.000000 pipsqlitedbextsV2-1.0.0/pipsqlitedbextsV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-16 20:10:05.000000 pipsqlitedbextsV2-1.0.0/pipsqlitedbextsV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 20:10:05.571380 pipsqlitedbextsV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-05-16 20:10:05.000000 pipsqlitedbextsV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:12:10.993859 pipsqlitedbextsV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-16 20:12:10.993859 pipsqlitedbextsV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:12:10.993859 pipsqlitedbextsV2-1.1.0/pipsqlitedbextsV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-16 20:12:10.000000 pipsqlitedbextsV2-1.1.0/pipsqlitedbextsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:12:10.993859 pipsqlitedbextsV2-1.1.0/pipsqlitedbextsV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-16 20:12:10.000000 pipsqlitedbextsV2-1.1.0/pipsqlitedbextsV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-16 20:12:10.000000 pipsqlitedbextsV2-1.1.0/pipsqlitedbextsV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 20:12:10.000000 pipsqlitedbextsV2-1.1.0/pipsqlitedbextsV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-16 20:12:10.000000 pipsqlitedbextsV2-1.1.0/pipsqlitedbextsV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 20:12:10.993859 pipsqlitedbextsV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-05-16 20:12:10.000000 pipsqlitedbextsV2-1.1.0/setup.py
```

### Comparing `pipsqlitedbextsV2-1.0.0/setup.py` & `pipsqlitedbextsV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipsqlitedbextsV2",
     version=VERSION,
```

