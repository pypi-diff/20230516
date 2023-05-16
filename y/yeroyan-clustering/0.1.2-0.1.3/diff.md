# Comparing `tmp/yeroyan_clustering-0.1.2.tar.gz` & `tmp/yeroyan_clustering-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeroyan_clustering-0.1.2.tar", last modified: Tue May 16 20:53:05 2023, max compression
+gzip compressed data, was "yeroyan_clustering-0.1.3.tar", last modified: Tue May 16 21:08:24 2023, max compression
```

## Comparing `yeroyan_clustering-0.1.2.tar` & `yeroyan_clustering-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 20:53:05.495547 yeroyan_clustering-0.1.2/
--rw-rw-rw-   0        0        0      171 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3744 2023-05-16 16:24:10.000000 yeroyan_clustering-0.1.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      246 2023-05-16 16:26:58.000000 yeroyan_clustering-0.1.2/HISTORY.rst
--rw-rw-rw-   0        0        0    11357 2023-05-08 20:04:04.000000 yeroyan_clustering-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      355 2023-05-16 20:47:19.000000 yeroyan_clustering-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1980 2023-05-16 20:53:05.495547 yeroyan_clustering-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 20:53:05.473384 yeroyan_clustering-0.1.2/docs/
--rw-rw-rw-   0        0        0      639 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/authors.rst
--rw-rw-rw-   0        0        0     5080 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/history.rst
--rw-rw-rw-   0        0        0      335 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/index.rst
--rw-rw-rw-   0        0        0     1265 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/installation.rst
--rwxrwxrwx   0        0        0      816 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/readme.rst
--rw-rw-rw-   0        0        0       98 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/docs/usage.rst
--rw-rw-rw-   0        0        0      461 2023-05-16 20:53:05.496547 yeroyan_clustering-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1255 2023-05-16 20:49:04.000000 yeroyan_clustering-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:53:05.475384 yeroyan_clustering-0.1.2/tests/
--rw-rw-rw-   0        0        0       49 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      941 2023-05-16 20:25:05.000000 yeroyan_clustering-0.1.2/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:53:05.477384 yeroyan_clustering-0.1.2/yeroyan_clustering/
--rw-rw-rw-   0        0        0      143 2023-05-16 20:49:04.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:53:05.489496 yeroyan_clustering-0.1.2/yeroyan_clustering/data/
--rw-rw-rw-   0        0        0    87208 2023-05-16 10:17:59.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/data/telco.csv
--rw-rw-rw-   0        0        0    60302 2023-05-16 14:24:50.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/data/titanic.csv
--rw-rw-rw-   0        0        0     1993 2023-05-16 20:24:04.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/main.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:53:05.491496 yeroyan_clustering-0.1.2/yeroyan_clustering/modeling/
--rw-rw-rw-   0        0        0      123 2023-05-16 19:22:34.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/modeling/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-05-16 19:21:19.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/modeling/base_models.py
--rw-rw-rw-   0        0        0     3149 2023-05-16 19:17:36.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/modeling/kmeans.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:53:05.492545 yeroyan_clustering-0.1.2/yeroyan_clustering/notebooks/
--rw-rw-rw-   0        0        0  1313986 2023-05-16 16:08:51.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/notebooks/analysis.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-16 20:53:05.495547 yeroyan_clustering-0.1.2/yeroyan_clustering/processing/
--rw-rw-rw-   0        0        0      203 2023-05-16 19:06:18.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/processing/__init__.py
--rw-rw-rw-   0        0        0    10619 2023-05-16 19:06:56.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/processing/dataset_processing.py
--rw-rw-rw-   0        0        0     4042 2023-05-16 19:07:29.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/processing/dimensionality_reduction.py
--rw-rw-rw-   0        0        0     2672 2023-05-16 19:32:29.000000 yeroyan_clustering-0.1.2/yeroyan_clustering/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:53:05.488498 yeroyan_clustering-0.1.2/yeroyan_clustering.egg-info/
--rw-rw-rw-   0        0        0     1980 2023-05-16 20:53:05.000000 yeroyan_clustering-0.1.2/yeroyan_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-05-16 20:53:05.000000 yeroyan_clustering-0.1.2/yeroyan_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:53:05.000000 yeroyan_clustering-0.1.2/yeroyan_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 20:53:05.000000 yeroyan_clustering-0.1.2/yeroyan_clustering.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2023-05-16 20:53:05.000000 yeroyan_clustering-0.1.2/yeroyan_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 21:08:24.396928 yeroyan_clustering-0.1.3/
+-rw-rw-rw-   0        0        0      171 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3744 2023-05-16 16:24:10.000000 yeroyan_clustering-0.1.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      246 2023-05-16 16:26:58.000000 yeroyan_clustering-0.1.3/HISTORY.rst
+-rw-rw-rw-   0        0        0    11357 2023-05-08 20:04:04.000000 yeroyan_clustering-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      355 2023-05-16 20:47:19.000000 yeroyan_clustering-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1980 2023-05-16 21:08:24.396928 yeroyan_clustering-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 21:08:24.371745 yeroyan_clustering-0.1.3/docs/
+-rw-rw-rw-   0        0        0      639 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/authors.rst
+-rw-rw-rw-   0        0        0     5080 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/history.rst
+-rw-rw-rw-   0        0        0      335 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1265 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/installation.rst
+-rwxrwxrwx   0        0        0      816 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/readme.rst
+-rw-rw-rw-   0        0        0       98 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/docs/usage.rst
+-rw-rw-rw-   0        0        0      461 2023-05-16 21:08:24.398927 yeroyan_clustering-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2023-05-16 21:07:58.000000 yeroyan_clustering-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:08:24.373748 yeroyan_clustering-0.1.3/tests/
+-rw-rw-rw-   0        0        0       49 2023-05-08 20:03:32.000000 yeroyan_clustering-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      941 2023-05-16 20:25:05.000000 yeroyan_clustering-0.1.3/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:08:24.375747 yeroyan_clustering-0.1.3/yeroyan_clustering/
+-rw-rw-rw-   0        0        0      143 2023-05-16 21:07:58.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:08:24.390860 yeroyan_clustering-0.1.3/yeroyan_clustering/data/
+-rw-rw-rw-   0        0        0    87208 2023-05-16 10:17:59.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/data/telco.csv
+-rw-rw-rw-   0        0        0    60302 2023-05-16 14:24:50.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/data/titanic.csv
+-rw-rw-rw-   0        0        0     1993 2023-05-16 20:24:04.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/main.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:08:24.392925 yeroyan_clustering-0.1.3/yeroyan_clustering/modeling/
+-rw-rw-rw-   0        0        0      123 2023-05-16 19:22:34.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/modeling/__init__.py
+-rw-rw-rw-   0        0        0     1588 2023-05-16 19:21:19.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/modeling/base_models.py
+-rw-rw-rw-   0        0        0     3149 2023-05-16 19:17:36.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/modeling/kmeans.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:08:24.392925 yeroyan_clustering-0.1.3/yeroyan_clustering/notebooks/
+-rw-rw-rw-   0        0        0  1313986 2023-05-16 16:08:51.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/notebooks/analysis.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-16 21:08:24.396928 yeroyan_clustering-0.1.3/yeroyan_clustering/processing/
+-rw-rw-rw-   0        0        0      203 2023-05-16 19:06:18.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/processing/__init__.py
+-rw-rw-rw-   0        0        0    10619 2023-05-16 19:06:56.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/processing/dataset_processing.py
+-rw-rw-rw-   0        0        0     4042 2023-05-16 19:07:29.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/processing/dimensionality_reduction.py
+-rw-rw-rw-   0        0        0     2672 2023-05-16 19:32:29.000000 yeroyan_clustering-0.1.3/yeroyan_clustering/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:08:24.388860 yeroyan_clustering-0.1.3/yeroyan_clustering.egg-info/
+-rw-rw-rw-   0        0        0     1980 2023-05-16 21:08:24.000000 yeroyan_clustering-0.1.3/yeroyan_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-05-16 21:08:24.000000 yeroyan_clustering-0.1.3/yeroyan_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:08:24.000000 yeroyan_clustering-0.1.3/yeroyan_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 21:08:24.000000 yeroyan_clustering-0.1.3/yeroyan_clustering.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-05-16 21:08:24.000000 yeroyan_clustering-0.1.3/yeroyan_clustering.egg-info/top_level.txt
```

### Comparing `yeroyan_clustering-0.1.2/CONTRIBUTING.rst` & `yeroyan_clustering-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/LICENSE` & `yeroyan_clustering-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/PKG-INFO` & `yeroyan_clustering-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeroyan_clustering
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automated Clustering and Anomaly Detection
 Home-page: https://github.com/Ara-Yeroyan/yeroyan_clustering
 Author: Ara Yeroyan
 Author-email: ar23yeroyan@gmail.com
 License: Apache Software License 2.0
 Keywords: yeroyan_clustering
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yeroyan_clustering-0.1.2/README.rst` & `yeroyan_clustering-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/docs/Makefile` & `yeroyan_clustering-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/docs/conf.py` & `yeroyan_clustering-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/docs/installation.rst` & `yeroyan_clustering-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/docs/make.bat` & `yeroyan_clustering-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/setup.py` & `yeroyan_clustering-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     include_package_data=True,
     keywords='yeroyan_clustering',
     name='yeroyan_clustering',
     packages=find_packages(include=['yeroyan_clustering', 'yeroyan_clustering.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Ara-Yeroyan/yeroyan_clustering',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `yeroyan_clustering-0.1.2/tests/test_main.py` & `yeroyan_clustering-0.1.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering/data/telco.csv` & `yeroyan_clustering-0.1.3/yeroyan_clustering/data/telco.csv`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering/data/titanic.csv` & `yeroyan_clustering-0.1.3/yeroyan_clustering/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering/main.py` & `yeroyan_clustering-0.1.3/yeroyan_clustering/main.py`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering/modeling/base_models.py` & `yeroyan_clustering-0.1.3/yeroyan_clustering/modeling/base_models.py`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering/modeling/kmeans.py` & `yeroyan_clustering-0.1.3/yeroyan_clustering/modeling/kmeans.py`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering/notebooks/analysis.ipynb` & `yeroyan_clustering-0.1.3/yeroyan_clustering/notebooks/analysis.ipynb`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering/processing/dataset_processing.py` & `yeroyan_clustering-0.1.3/yeroyan_clustering/processing/dataset_processing.py`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering/processing/dimensionality_reduction.py` & `yeroyan_clustering-0.1.3/yeroyan_clustering/processing/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering/utils.py` & `yeroyan_clustering-0.1.3/yeroyan_clustering/utils.py`

 * *Files identical despite different names*

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering.egg-info/PKG-INFO` & `yeroyan_clustering-0.1.3/yeroyan_clustering.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeroyan-clustering
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automated Clustering and Anomaly Detection
 Home-page: https://github.com/Ara-Yeroyan/yeroyan_clustering
 Author: Ara Yeroyan
 Author-email: ar23yeroyan@gmail.com
 License: Apache Software License 2.0
 Keywords: yeroyan_clustering
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yeroyan_clustering-0.1.2/yeroyan_clustering.egg-info/SOURCES.txt` & `yeroyan_clustering-0.1.3/yeroyan_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

