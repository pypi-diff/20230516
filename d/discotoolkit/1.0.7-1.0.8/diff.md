# Comparing `tmp/discotoolkit-1.0.7.tar.gz` & `tmp/discotoolkit-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.0.7.tar", last modified: Mon May 15 13:44:16 2023, max compression
+gzip compressed data, was "discotoolkit-1.0.8.tar", last modified: Tue May 16 06:03:22 2023, max compression
```

## Comparing `discotoolkit-1.0.7.tar` & `discotoolkit-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-15 13:44:05.588393 discotoolkit-1.0.7/
--rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.7/MANIFEST.in
--rw-rw-r--   0 rom       (1013) rom       (1027)      689 2023-05-15 13:44:05.588393 discotoolkit-1.0.7/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)     2366 2023-05-15 13:43:25.000000 discotoolkit-1.0.7/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-15 13:44:05.548393 discotoolkit-1.0.7/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)    17688 2023-05-15 11:46:41.000000 discotoolkit-1.0.7/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.7/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     2498 2023-05-13 12:39:48.000000 discotoolkit-1.0.7/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     7377 2023-05-15 05:29:07.000000 discotoolkit-1.0.7/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.0.7/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.0.7/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      130 2023-05-15 13:43:45.000000 discotoolkit-1.0.7/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-15 13:44:05.580393 discotoolkit-1.0.7/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      689 2023-05-15 13:44:05.000000 discotoolkit-1.0.7/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-15 13:44:05.000000 discotoolkit-1.0.7/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-15 13:44:05.000000 discotoolkit-1.0.7/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)      246 2023-05-15 13:44:05.000000 discotoolkit-1.0.7/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-15 13:44:05.000000 discotoolkit-1.0.7/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-15 13:44:05.592393 discotoolkit-1.0.7/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)     1135 2023-05-15 13:41:38.000000 discotoolkit-1.0.7/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-16 06:03:11.017838 discotoolkit-1.0.8/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.8/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-16 06:03:11.013838 discotoolkit-1.0.8/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2599 2023-05-16 06:01:24.000000 discotoolkit-1.0.8/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-16 06:03:10.973838 discotoolkit-1.0.8/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)    17688 2023-05-16 05:02:50.000000 discotoolkit-1.0.8/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.8/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2498 2023-05-13 12:39:48.000000 discotoolkit-1.0.8/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     7377 2023-05-15 05:29:07.000000 discotoolkit-1.0.8/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-12 05:21:05.000000 discotoolkit-1.0.8/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-11 01:48:58.000000 discotoolkit-1.0.8/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      130 2023-05-16 06:01:49.000000 discotoolkit-1.0.8/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-16 06:03:11.005838 discotoolkit-1.0.8/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      679 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)      106 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-16 06:03:10.000000 discotoolkit-1.0.8/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-16 06:03:11.017838 discotoolkit-1.0.8/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1052 2023-05-16 06:02:14.000000 discotoolkit-1.0.8/setup.py
```

### Comparing `discotoolkit-1.0.7/PKG-INFO` & `discotoolkit-1.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.7
+Version: 1.0.8
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 Requires-Python: >=3.8.16
 
-
-    DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
-    
-
-    Filter and download DISCO data based on sample metadata and cell type information
-    
-CELLiD: cell type annotation
-    
+DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.         It provides the following functions
+Filter and download DISCO data based on sample metadata and cell type information
+CELLiD:             cell type annotation
 scEnrichment: geneset enrichment using DISCO DEGs
-
```

### Comparing `discotoolkit-1.0.7/README.md` & `discotoolkit-1.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
  * @Descripttion: 
  * @version: 
  * @Author: Mengwei Li
  * @Date: 2023-04-16 21:20:42
  * @LastEditors: Mengwei Li
  * @LastEditTime: 2023-04-16 21:22:03
 -->
-[![Documentation Status](https://readthedocs.org/projects/discotoolkit-py/badge/?version=latest)](https://discotoolkit-py.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/discotoolkit?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/discotoolkit)
+[![Documentation Status](https://readthedocs.org/projects/discotoolkit-py/badge/?version=latest)](https://discotoolkit-py.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/discotoolkit?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/discotoolkit) [![PyPI version](https://img.shields.io/pypi/v/discotoolkit)](https://pypi.org/project/discotoolkit)
 
-# DISCOtoolkit 1.0.7
+# DISCOtoolkit 1.0.8
 
 DISCOtoolkit is an python package that allows users to access data and use the tools provided by the [DISCO database](https://www.immunesinglecell.org/). Read the documentation [DISCOtoolkit](https://discotoolkit-py.readthedocs.io/en/latest/). It provides the following functions:
 
 - Filter and download DISCO data based on sample metadata and cell type information
 - CELLiD: cell type annotation
 - scEnrichment: geneset enrichment using DISCO DEGs
 
@@ -25,18 +25,28 @@
 - joblib >= 1.1.0
 - pandarallel >= 1.6.5
 
 ## Installation guide:
 
 we recommend to install miniconda first and install discotoolkit in virtual env
 
+## Installation guide:
+
+we recommend to install miniconda first and install discotoolkit in virtual env
+
 ```
 conda create --name disco python=3.8
-conda install pip
+```
+```
+conda activate disco
+```
+```
 conda install ipykernel
+```
+```
 python -m ipykernel install --user --name disco --display-name "disco"
 ```
 
 Installation using pip:
 ``` 
 python -m pip install discotoolkit # adding -U for installing the latest version
 ```
```

### Comparing `discotoolkit-1.0.7/discotoolkit/CELLiD.py` & `discotoolkit-1.0.8/discotoolkit/CELLiD.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.7/discotoolkit/DiscoClass.py` & `discotoolkit-1.0.8/discotoolkit/DiscoClass.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.7/discotoolkit/DownloadDiscoData.py` & `discotoolkit-1.0.8/discotoolkit/DownloadDiscoData.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.7/discotoolkit/GetMetadata.py` & `discotoolkit-1.0.8/discotoolkit/GetMetadata.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.7/discotoolkit/GlobalVariable.py` & `discotoolkit-1.0.8/discotoolkit/GlobalVariable.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0.7/discotoolkit.egg-info/PKG-INFO` & `discotoolkit-1.0.8/discotoolkit.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.7
+Version: 1.0.8
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 Requires-Python: >=3.8.16
 
-
-    DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
-    
-
-    Filter and download DISCO data based on sample metadata and cell type information
-    
-CELLiD: cell type annotation
-    
+DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.         It provides the following functions
+Filter and download DISCO data based on sample metadata and cell type information
+CELLiD:             cell type annotation
 scEnrichment: geneset enrichment using DISCO DEGs
-
```

### Comparing `discotoolkit-1.0.7/setup.py` & `discotoolkit-1.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 from setuptools import setup, find_packages
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
-with open('docs/version.txt', 'r') as f:
-    version = f.read().strip()
-
 setup(
     name='discotoolkit',
-    version=version,
+    version="1.0.8",
     url='http://www.immunesinglecell.org/',
     author='Li Mengwei, Rom Uddamvathanak',
     author_email='uddamvathanak_rom@immunol.a-star.edu.sg',
     description='DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.',
     packages=find_packages(include=["discotoolkit", "discotoolkit.*"]),
     install_requires=requirements,
     python_requires = '>=3.8.16',
     include_package_data=True,
-    long_description="""
-    DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
-    \n
-    Filter and download DISCO data based on sample metadata and cell type information
-    \nCELLiD: cell type annotation
-    \nscEnrichment: geneset enrichment using DISCO DEGs
-    """,
+    long_description="DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. \
+        It provides the following functions\nFilter and download DISCO data based on sample metadata and cell type information\nCELLiD: \
+            cell type annotation\nscEnrichment: geneset enrichment using DISCO DEGs",
 )
```

