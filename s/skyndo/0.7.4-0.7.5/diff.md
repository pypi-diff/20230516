# Comparing `tmp/skyndo-0.7.4.tar.gz` & `tmp/skyndo-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyndo-0.7.4.tar", last modified: Tue May 16 07:47:53 2023, max compression
+gzip compressed data, was "skyndo-0.7.5.tar", last modified: Tue May 16 07:51:11 2023, max compression
```

## Comparing `skyndo-0.7.4.tar` & `skyndo-0.7.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:47:53.776770 skyndo-0.7.4/
--rw-rw-rw-   0        0        0      378 2023-05-16 07:47:53.775710 skyndo-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-16 07:47:53.776770 skyndo-0.7.4/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-05-16 07:46:59.000000 skyndo-0.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:47:53.738232 skyndo-0.7.4/skyndo/
--rw-rw-rw-   0        0        0        0 2023-03-31 15:55:53.000000 skyndo-0.7.4/skyndo/_init_.py
--rw-rw-rw-   0        0        0     2175 2023-05-16 04:33:41.000000 skyndo-0.7.4/skyndo/predict.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:47:53.773716 skyndo-0.7.4/skyndo.egg-info/
--rw-rw-rw-   0        0        0      378 2023-05-16 07:47:51.000000 skyndo-0.7.4/skyndo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-05-16 07:47:53.000000 skyndo-0.7.4/skyndo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:47:51.000000 skyndo-0.7.4/skyndo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-16 07:47:51.000000 skyndo-0.7.4/skyndo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 07:47:51.000000 skyndo-0.7.4/skyndo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 07:51:11.464122 skyndo-0.7.5/
+-rw-rw-rw-   0        0        0      378 2023-05-16 07:51:11.462484 skyndo-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:51:11.465207 skyndo-0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0      568 2023-05-16 07:50:33.000000 skyndo-0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:51:11.355744 skyndo-0.7.5/skyndo/
+-rw-rw-rw-   0        0        0        0 2023-03-31 15:55:53.000000 skyndo-0.7.5/skyndo/_init_.py
+-rw-rw-rw-   0        0        0     2175 2023-05-16 04:33:41.000000 skyndo-0.7.5/skyndo/predict.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:51:11.460971 skyndo-0.7.5/skyndo.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-05-16 07:51:09.000000 skyndo-0.7.5/skyndo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-16 07:51:10.000000 skyndo-0.7.5/skyndo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:51:09.000000 skyndo-0.7.5/skyndo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-16 07:51:09.000000 skyndo-0.7.5/skyndo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 07:51:09.000000 skyndo-0.7.5/skyndo.egg-info/top_level.txt
```

### Comparing `skyndo-0.7.4/setup.py` & `skyndo-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='skyndo',
-    version='0.7.4',
+    version='0.7.5',
     packages=['skyndo'],
     include_data=True,
     data= ('data', ['model.pkl']),
     install_requires=[
         'pandas',
         'scikit-learn',
         'numpy'],
```

### Comparing `skyndo-0.7.4/skyndo/predict.py` & `skyndo-0.7.5/skyndo/predict.py`

 * *Files identical despite different names*

