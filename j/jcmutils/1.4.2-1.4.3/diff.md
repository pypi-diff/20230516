# Comparing `tmp/jcmutils-1.4.2.tar.gz` & `tmp/jcmutils-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.4.2.tar", last modified: Thu May 11 10:06:52 2023, max compression
+gzip compressed data, was "jcmutils-1.4.3.tar", last modified: Tue May 16 07:28:09 2023, max compression
```

## Comparing `jcmutils-1.4.2.tar` & `jcmutils-1.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-11 10:06:52.483250 jcmutils-1.4.2/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.2/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-11 10:06:52.483250 jcmutils-1.4.2/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.2/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-11 10:06:52.483250 jcmutils-1.4.2/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.2/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2613 2023-04-19 07:20:15.000000 jcmutils-1.4.2/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.2/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.2/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-11 10:05:05.000000 jcmutils-1.4.2/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-11 10:06:52.483250 jcmutils-1.4.2/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-11 10:06:52.000000 jcmutils-1.4.2/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-11 10:06:52.483250 jcmutils-1.4.2/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-05-11 10:05:31.000000 jcmutils-1.4.2/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-16 07:28:09.165178 jcmutils-1.4.3/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.3/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-16 07:28:09.165178 jcmutils-1.4.3/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.3/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-16 07:28:09.165178 jcmutils-1.4.3/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.3/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     6777 2023-05-16 07:27:18.000000 jcmutils-1.4.3/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.3/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.3/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-11 10:05:05.000000 jcmutils-1.4.3/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-16 07:28:09.165178 jcmutils-1.4.3/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-16 07:28:09.165178 jcmutils-1.4.3/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-16 07:27:37.000000 jcmutils-1.4.3/setup.py
```

### Comparing `jcmutils-1.4.2/LICENSE` & `jcmutils-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.2/README.md` & `jcmutils-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.2/jcmutils/gen_sources.py` & `jcmutils-1.4.3/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.2/jcmutils/logger.py` & `jcmutils-1.4.3/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.2/jcmutils/solver.py` & `jcmutils-1.4.3/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.2/setup.py` & `jcmutils-1.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.4.2'
+VERSION = '1.4.3'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=["numpy","matplotlib","opencv-python"],
+    install_requires=["numpy","matplotlib","opencv-python","pyyaml"],
     keywords=["jcmsuite","utils"],
     classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     ]
 )
```

