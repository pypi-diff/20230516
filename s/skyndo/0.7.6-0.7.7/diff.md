# Comparing `tmp/skyndo-0.7.6.tar.gz` & `tmp/skyndo-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyndo-0.7.6.tar", last modified: Tue May 16 08:01:16 2023, max compression
+gzip compressed data, was "skyndo-0.7.7.tar", last modified: Tue May 16 08:27:11 2023, max compression
```

## Comparing `skyndo-0.7.6.tar` & `skyndo-0.7.7.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:01:16.143735 skyndo-0.7.6/
--rw-rw-rw-   0        0        0      378 2023-05-16 08:01:16.128774 skyndo-0.7.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 08:01:15.692739 skyndo-0.7.6/data/
--rw-rw-rw-   0        0        0 25199035 2023-03-31 16:13:20.000000 skyndo-0.7.6/data/model.pkl
--rw-rw-rw-   0        0        0       42 2023-05-16 08:01:16.143735 skyndo-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0      599 2023-05-16 07:58:08.000000 skyndo-0.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:01:16.058257 skyndo-0.7.6/skyndo/
--rw-rw-rw-   0        0        0        0 2023-03-31 15:55:53.000000 skyndo-0.7.6/skyndo/_init_.py
--rw-rw-rw-   0        0        0     2175 2023-05-16 04:33:41.000000 skyndo-0.7.6/skyndo/predict.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:01:16.126780 skyndo-0.7.6/skyndo.egg-info/
--rw-rw-rw-   0        0        0      378 2023-05-16 08:01:13.000000 skyndo-0.7.6/skyndo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-16 08:01:13.000000 skyndo-0.7.6/skyndo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:01:13.000000 skyndo-0.7.6/skyndo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-16 08:01:13.000000 skyndo-0.7.6/skyndo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 08:01:13.000000 skyndo-0.7.6/skyndo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 08:27:11.938663 skyndo-0.7.7/
+-rw-rw-rw-   0        0        0      378 2023-05-16 08:27:11.937666 skyndo-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:27:11.938663 skyndo-0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-05-16 08:26:07.000000 skyndo-0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:27:10.094596 skyndo-0.7.7/skyndo/
+-rw-rw-rw-   0        0        0        0 2023-03-31 15:55:53.000000 skyndo-0.7.7/skyndo/_init_.py
+-rw-rw-rw-   0        0        0     2175 2023-05-16 04:33:41.000000 skyndo-0.7.7/skyndo/predict.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:27:11.935672 skyndo-0.7.7/skyndo.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-05-16 08:27:09.000000 skyndo-0.7.7/skyndo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-16 08:27:09.000000 skyndo-0.7.7/skyndo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:27:09.000000 skyndo-0.7.7/skyndo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-16 08:27:09.000000 skyndo-0.7.7/skyndo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 08:27:09.000000 skyndo-0.7.7/skyndo.egg-info/top_level.txt
```

### Comparing `skyndo-0.7.6/setup.py` & `skyndo-0.7.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='skyndo',
-    version='0.7.6',
+    version='0.7.7',
     packages=['skyndo'],
     include_data=True,
     data_files = [
-        ('data', ['data/model.pkl']),
+        ('skyndo', ['model.pkl']),
     ],
     install_requires=[
         'pandas',
         'scikit-learn',
         'numpy'],
     author='Nishan Obeyesekera',
     author_email='nishandhanu21@gmail.com',
```

### Comparing `skyndo-0.7.6/skyndo/predict.py` & `skyndo-0.7.7/skyndo/predict.py`

 * *Files identical despite different names*

