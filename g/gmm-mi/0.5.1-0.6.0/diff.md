# Comparing `tmp/gmm_mi-0.5.1.tar.gz` & `tmp/gmm_mi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmm_mi-0.5.1.tar", last modified: Sun May 14 22:30:32 2023, max compression
+gzip compressed data, was "gmm_mi-0.6.0.tar", last modified: Mon May 15 22:09:15 2023, max compression
```

## Comparing `gmm_mi-0.5.1.tar` & `gmm_mi-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-14 22:30:32.422691 gmm_mi-0.5.1/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.5.1/LICENSE.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.5.1/LICENSE_EXT.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-05-14 22:30:32.421691 gmm_mi-0.5.1/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10270 2023-05-14 15:46:30.000000 gmm_mi-0.5.1/README.md
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-14 22:30:32.357690 gmm_mi-0.5.1/gmm_mi/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.5.1/gmm_mi/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.5.1/gmm_mi/cross_validation.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-14 22:30:32.373690 gmm_mi-0.5.1/gmm_mi/data/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.5.1/gmm_mi/data/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.5.1/gmm_mi/data/synthetic_data.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    24708 2023-05-14 14:04:14.000000 gmm_mi-0.5.1/gmm_mi/gmm.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.5.1/gmm_mi/initializations.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    45340 2023-05-14 14:09:38.000000 gmm_mi-0.5.1/gmm_mi/mi.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.5.1/gmm_mi/param_holders.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.5.1/gmm_mi/single_fit.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-14 22:30:32.413691 gmm_mi-0.5.1/gmm_mi/utils/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.5.1/gmm_mi/utils/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.5.1/gmm_mi/utils/analytic_MI.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    29790 2023-01-04 21:01:21.000000 gmm_mi-0.5.1/gmm_mi/utils/plotting.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.5.1/gmm_mi/utils/transformations.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-14 22:30:32.369691 gmm_mi-0.5.1/gmm_mi.egg-info/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-05-14 22:30:32.000000 gmm_mi-0.5.1/gmm_mi.egg-info/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-05-14 22:30:32.000000 gmm_mi-0.5.1/gmm_mi.egg-info/SOURCES.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-05-14 22:30:32.000000 gmm_mi-0.5.1/gmm_mi.egg-info/dependency_links.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-05-14 22:30:32.000000 gmm_mi-0.5.1/gmm_mi.egg-info/requires.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-05-14 22:30:32.000000 gmm_mi-0.5.1/gmm_mi.egg-info/top_level.txt
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-14 22:30:32.419691 gmm_mi-0.5.1/notebooks/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.5.1/notebooks/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-05-14 22:30:32.422691 gmm_mi-0.5.1/setup.cfg
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-05-14 15:45:33.000000 gmm_mi-0.5.1/setup.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.983382 gmm_mi-0.6.0/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.6.0/LICENSE.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.6.0/LICENSE_EXT.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-05-15 22:09:14.973382 gmm_mi-0.6.0/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10270 2023-05-14 15:46:30.000000 gmm_mi-0.6.0/README.md
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.834382 gmm_mi-0.6.0/gmm_mi/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.6.0/gmm_mi/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.6.0/gmm_mi/cross_validation.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.868382 gmm_mi-0.6.0/gmm_mi/data/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.6.0/gmm_mi/data/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.6.0/gmm_mi/data/synthetic_data.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    24708 2023-05-14 14:04:14.000000 gmm_mi-0.6.0/gmm_mi/gmm.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.6.0/gmm_mi/initializations.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    45340 2023-05-14 14:09:38.000000 gmm_mi-0.6.0/gmm_mi/mi.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.6.0/gmm_mi/param_holders.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.6.0/gmm_mi/single_fit.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.924382 gmm_mi-0.6.0/gmm_mi/utils/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.6.0/gmm_mi/utils/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.6.0/gmm_mi/utils/analytic_MI.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    29790 2023-01-04 21:01:21.000000 gmm_mi-0.6.0/gmm_mi/utils/plotting.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.6.0/gmm_mi/utils/transformations.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.859382 gmm_mi-0.6.0/gmm_mi.egg-info/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/requires.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-05-15 22:09:14.000000 gmm_mi-0.6.0/gmm_mi.egg-info/top_level.txt
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-05-15 22:09:14.955382 gmm_mi-0.6.0/notebooks/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.6.0/notebooks/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-05-15 22:09:14.985382 gmm_mi-0.6.0/setup.cfg
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-05-15 10:31:27.000000 gmm_mi-0.6.0/setup.py
```

### Comparing `gmm_mi-0.5.1/LICENSE.txt` & `gmm_mi-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/LICENSE_EXT.txt` & `gmm_mi-0.6.0/LICENSE_EXT.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/PKG-INFO` & `gmm_mi-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm_mi
-Version: 0.5.1
+Version: 0.6.0
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gmm_mi-0.5.1/README.md` & `gmm_mi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/cross_validation.py` & `gmm_mi-0.6.0/gmm_mi/cross_validation.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/data/synthetic_data.py` & `gmm_mi-0.6.0/gmm_mi/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/gmm.py` & `gmm_mi-0.6.0/gmm_mi/gmm.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/initializations.py` & `gmm_mi-0.6.0/gmm_mi/initializations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/mi.py` & `gmm_mi-0.6.0/gmm_mi/mi.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/param_holders.py` & `gmm_mi-0.6.0/gmm_mi/param_holders.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/single_fit.py` & `gmm_mi-0.6.0/gmm_mi/single_fit.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/utils/analytic_MI.py` & `gmm_mi-0.6.0/gmm_mi/utils/analytic_MI.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/utils/plotting.py` & `gmm_mi-0.6.0/gmm_mi/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi/utils/transformations.py` & `gmm_mi-0.6.0/gmm_mi/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/gmm_mi.egg-info/PKG-INFO` & `gmm_mi-0.6.0/gmm_mi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm-mi
-Version: 0.5.1
+Version: 0.6.0
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gmm_mi-0.5.1/gmm_mi.egg-info/SOURCES.txt` & `gmm_mi-0.6.0/gmm_mi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.5.1/setup.py` & `gmm_mi-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 PACKAGENAME = 'gmm_mi'
 
 setup(
     name='gmm_mi',
-    version="0.5.1",
+    version="0.6.0",
     author='Davide Piras',
     author_email='dr.davide.piras@gmail.com',
     description='Estimate mutual information distribution with Gaussian mixture models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dpiras/GMM-MI',
     license='GNU General Public License v3.0 (GPLv3)',
```

