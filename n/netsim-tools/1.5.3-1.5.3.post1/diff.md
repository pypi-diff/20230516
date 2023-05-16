# Comparing `tmp/netsim-tools-1.5.3.tar.gz` & `tmp/netsim-tools-1.5.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsim-tools-1.5.3.tar", last modified: Mon May 15 07:02:14 2023, max compression
+gzip compressed data, was "netsim-tools-1.5.3.post1.tar", last modified: Tue May 16 06:09:07 2023, max compression
```

## Comparing `netsim-tools-1.5.3.tar` & `netsim-tools-1.5.3.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-15 07:02:14.682267 netsim-tools-1.5.3/
--rw-r--r--   0 pipi       (501) staff       (20)      493 2023-05-15 07:02:14.682147 netsim-tools-1.5.3/PKG-INFO
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-15 07:02:14.681985 netsim-tools-1.5.3/netsim_tools.egg-info/
--rw-r--r--   0 pipi       (501) staff       (20)      493 2023-05-15 07:02:14.000000 netsim-tools-1.5.3/netsim_tools.egg-info/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)      187 2023-05-15 07:02:14.000000 netsim-tools-1.5.3/netsim_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-05-15 07:02:14.000000 netsim-tools-1.5.3/netsim_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pipi       (501) staff       (20)       18 2023-05-15 07:02:14.000000 netsim-tools-1.5.3/netsim_tools.egg-info/requires.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-05-15 07:02:14.000000 netsim-tools-1.5.3/netsim_tools.egg-info/top_level.txt
--rw-r--r--   0 pipi       (501) staff       (20)       38 2023-05-15 07:02:14.682298 netsim-tools-1.5.3/setup.cfg
--rw-r--r--   0 pipi       (501) staff       (20)     1292 2023-05-15 06:46:09.000000 netsim-tools-1.5.3/setup.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:09:07.576027 netsim-tools-1.5.3.post1/
+-rw-r--r--   0 pipi       (501) staff       (20)      499 2023-05-16 06:09:07.575914 netsim-tools-1.5.3.post1/PKG-INFO
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:09:07.575770 netsim-tools-1.5.3.post1/netsim_tools.egg-info/
+-rw-r--r--   0 pipi       (501) staff       (20)      499 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)      187 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        1 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       24 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/requires.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        1 2023-05-16 06:09:07.000000 netsim-tools-1.5.3.post1/netsim_tools.egg-info/top_level.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       38 2023-05-16 06:09:07.576065 netsim-tools-1.5.3.post1/setup.cfg
+-rw-r--r--   0 pipi       (501) staff       (20)     1298 2023-05-16 06:07:28.000000 netsim-tools-1.5.3.post1/setup.py
```

### Comparing `netsim-tools-1.5.3/setup.py` & `netsim-tools-1.5.3.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ redirect netsim-tools to networklab """
 import sys
 from setuptools import setup, find_packages
 
 sys.path.append('..')
 
-version="1.5.3"
+version="1.5.3-post1"
 
 setup(
   name="netsim-tools",
   version=version,
   packages=[],
   author="Ivan Pepelnjak",
   author_email="ip@ipspace.net",
```

