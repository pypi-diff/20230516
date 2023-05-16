# Comparing `tmp/BLiC-2023.2.0.tar.gz` & `tmp/BLiC-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BLiC-2023.2.0.tar", last modified: Mon Feb 27 14:10:45 2023, max compression
+gzip compressed data, was "dist/BLiC-2023.5.0.tar", last modified: Tue May 16 12:45:04 2023, max compression
```

## Comparing `BLiC-2023.2.0.tar` & `BLiC-2023.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zltan     (1023) jxhan     (1005)        0 2023-02-27 14:10:45.000000 BLiC-2023.2.0/
--rw-r--r--   0 zltan     (1023) jxhan     (1005)       77 2023-02-27 14:04:08.000000 BLiC-2023.2.0/README.md
--rw-r--r--   0 zltan     (1023) jxhan     (1005)     1064 2023-02-27 14:03:02.000000 BLiC-2023.2.0/LICENSE
--rw-r--r--   0 zltan     (1023) jxhan     (1005)      547 2023-02-27 14:10:45.000000 BLiC-2023.2.0/PKG-INFO
--rw-r--r--   0 zltan     (1023) jxhan     (1005)      598 2023-02-27 14:10:12.000000 BLiC-2023.2.0/setup.py
--rw-r--r--   0 zltan     (1023) jxhan     (1005)       38 2023-02-27 14:10:45.000000 BLiC-2023.2.0/setup.cfg
-drwxr-xr-x   0 zltan     (1023) jxhan     (1005)        0 2023-02-27 14:10:45.000000 BLiC-2023.2.0/BLiC.egg-info/
--rw-r--r--   0 zltan     (1023) jxhan     (1005)      370 2023-02-27 14:10:45.000000 BLiC-2023.2.0/BLiC.egg-info/SOURCES.txt
--rw-r--r--   0 zltan     (1023) jxhan     (1005)        1 2023-02-27 14:10:45.000000 BLiC-2023.2.0/BLiC.egg-info/top_level.txt
--rw-r--r--   0 zltan     (1023) jxhan     (1005)      547 2023-02-27 14:10:45.000000 BLiC-2023.2.0/BLiC.egg-info/PKG-INFO
-drwxr-xr-x   0 zltan     (1023) jxhan     (1005)        0 2023-02-27 14:10:45.000000 BLiC-2023.2.0/BLiC.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 zltan     (1023) jxhan     (1005)      138 2023-02-27 14:08:31.000000 BLiC-2023.2.0/BLiC.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 zltan     (1023) jxhan     (1005)        1 2023-02-27 14:08:31.000000 BLiC-2023.2.0/BLiC.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 zltan     (1023) jxhan     (1005)      552 2023-02-27 14:08:31.000000 BLiC-2023.2.0/BLiC.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 zltan     (1023) jxhan     (1005)        1 2023-02-27 14:08:31.000000 BLiC-2023.2.0/BLiC.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 zltan     (1023) jxhan     (1005)        1 2023-02-27 14:10:45.000000 BLiC-2023.2.0/BLiC.egg-info/dependency_links.txt
+drwxr-xr-x   0 zltan     (1023) jxhan     (1005)        0 2023-05-16 12:45:04.000000 BLiC-2023.5.0/
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)      260 2023-05-16 12:39:34.000000 BLiC-2023.5.0/README.md
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)     1064 2023-02-27 14:03:02.000000 BLiC-2023.5.0/LICENSE
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)      742 2023-05-16 12:45:04.000000 BLiC-2023.5.0/PKG-INFO
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)      610 2023-05-16 12:40:39.000000 BLiC-2023.5.0/setup.py
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)       38 2023-05-16 12:45:04.000000 BLiC-2023.5.0/setup.cfg
+drwxr-xr-x   0 zltan     (1023) jxhan     (1005)        0 2023-05-16 12:45:04.000000 BLiC-2023.5.0/BLiC.egg-info/
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)      370 2023-05-16 12:44:59.000000 BLiC-2023.5.0/BLiC.egg-info/SOURCES.txt
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)        1 2023-05-16 12:44:59.000000 BLiC-2023.5.0/BLiC.egg-info/top_level.txt
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)      742 2023-05-16 12:44:59.000000 BLiC-2023.5.0/BLiC.egg-info/PKG-INFO
+drwxr-xr-x   0 zltan     (1023) jxhan     (1005)        0 2023-05-16 12:45:04.000000 BLiC-2023.5.0/BLiC.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)      138 2023-02-27 14:08:31.000000 BLiC-2023.5.0/BLiC.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)        1 2023-02-27 14:08:31.000000 BLiC-2023.5.0/BLiC.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)      552 2023-02-27 14:08:31.000000 BLiC-2023.5.0/BLiC.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)        1 2023-02-27 14:08:31.000000 BLiC-2023.5.0/BLiC.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 zltan     (1023) jxhan     (1005)        1 2023-05-16 12:44:59.000000 BLiC-2023.5.0/BLiC.egg-info/dependency_links.txt
```

### Comparing `BLiC-2023.2.0/LICENSE` & `BLiC-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BLiC-2023.2.0/PKG-INFO` & `BLiC-2023.5.0/BLiC.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: BLiC
 Version: 2023.2.0
 Summary: A python package to Build Light-cones and output mock Catalogues
-Home-page: https://github.com/zltan000/BLiC
+Home-page: https://github.com/pypa/sampleproject
 Author: Zhenlin Tan
 Author-email: zltan999@sjtu.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `BLiC-2023.2.0/setup.py` & `BLiC-2023.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r") as f:
   long_description = f.read()
 
 setuptools.setup(
   name="BLiC",
-  version="2023.2.0",
-  author="Zhenlin Tan",
+  version="2023.5.0",
+  author="Zhenlin Tan, Jiaxin Han",
   author_email="zltan999@sjtu.edu.cn",
   description="A python package to Build Light-cones and output mock Catalogues",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/zltan000/BLiC",
   packages=setuptools.find_packages(),
   classifiers=[
```

