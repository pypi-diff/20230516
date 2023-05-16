# Comparing `tmp/scMet-1.0.1.tar.gz` & `tmp/scMet-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scMet-1.0.1.tar", last modified: Tue May 16 07:03:01 2023, max compression
+gzip compressed data, was "scMet-1.0.2.tar", last modified: Tue May 16 07:14:42 2023, max compression
```

## Comparing `scMet-1.0.1.tar` & `scMet-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:03:01.732869 scMet-1.0.1/
--rw-rw-rw-   0        0        0     1072 2023-05-16 02:09:26.000000 scMet-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       31 2023-05-16 06:39:45.000000 scMet-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      386 2023-05-16 07:03:01.731869 scMet-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-05-16 06:34:54.000000 scMet-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 07:03:01.699876 scMet-1.0.1/scMet/
--rw-rw-rw-   0        0        0    10060 2023-05-15 09:01:49.000000 scMet-1.0.1/scMet/CVAEmodel.py
--rw-rw-rw-   0        0        0     3257 2023-05-15 10:41:51.000000 scMet-1.0.1/scMet/Dataloader.py
--rw-rw-rw-   0        0        0     5061 2023-05-15 08:29:36.000000 scMet-1.0.1/scMet/Deconvolution.py
--rw-rw-rw-   0        0        0    10401 2023-05-15 08:29:36.000000 scMet-1.0.1/scMet/GenerateData.py
--rw-rw-rw-   0        0        0     8181 2023-05-16 01:59:56.000000 scMet-1.0.1/scMet/Main.py
--rw-rw-rw-   0        0        0     5505 2023-05-16 02:12:26.000000 scMet-1.0.1/scMet/Simulation.py
--rw-rw-rw-   0        0        0     6842 2023-05-16 02:07:09.000000 scMet-1.0.1/scMet/Std_choose.py
--rw-rw-rw-   0        0        0        0 2023-05-15 10:49:37.000000 scMet-1.0.1/scMet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:03:01.729858 scMet-1.0.1/scMet.egg-info/
--rw-rw-rw-   0        0        0      386 2023-05-16 07:03:01.000000 scMet-1.0.1/scMet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-05-16 07:03:01.000000 scMet-1.0.1/scMet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:03:01.000000 scMet-1.0.1/scMet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-05-16 07:03:01.000000 scMet-1.0.1/scMet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 07:03:01.000000 scMet-1.0.1/scMet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 07:03:01.732869 scMet-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      830 2023-05-16 07:02:55.000000 scMet-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:14:42.026587 scMet-1.0.2/
+-rw-rw-rw-   0        0        0     1072 2023-05-16 02:09:26.000000 scMet-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       31 2023-05-16 06:39:45.000000 scMet-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      386 2023-05-16 07:14:42.026587 scMet-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-05-16 06:34:54.000000 scMet-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 07:14:41.997604 scMet-1.0.2/scMet/
+-rw-rw-rw-   0        0        0    10060 2023-05-15 09:01:49.000000 scMet-1.0.2/scMet/CVAEmodel.py
+-rw-rw-rw-   0        0        0     3257 2023-05-15 10:41:51.000000 scMet-1.0.2/scMet/Dataloader.py
+-rw-rw-rw-   0        0        0     5061 2023-05-15 08:29:36.000000 scMet-1.0.2/scMet/Deconvolution.py
+-rw-rw-rw-   0        0        0    10401 2023-05-15 08:29:36.000000 scMet-1.0.2/scMet/GenerateData.py
+-rw-rw-rw-   0        0        0     8181 2023-05-16 01:59:56.000000 scMet-1.0.2/scMet/Main.py
+-rw-rw-rw-   0        0        0     5505 2023-05-16 02:12:26.000000 scMet-1.0.2/scMet/Simulation.py
+-rw-rw-rw-   0        0        0     6842 2023-05-16 02:07:09.000000 scMet-1.0.2/scMet/Std_choose.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:49:37.000000 scMet-1.0.2/scMet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:14:42.023610 scMet-1.0.2/scMet.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-05-16 07:14:41.000000 scMet-1.0.2/scMet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-05-16 07:14:41.000000 scMet-1.0.2/scMet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:14:41.000000 scMet-1.0.2/scMet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-16 07:14:41.000000 scMet-1.0.2/scMet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-16 07:14:41.000000 scMet-1.0.2/scMet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:14:42.026587 scMet-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-05-16 07:14:23.000000 scMet-1.0.2/setup.py
```

### Comparing `scMet-1.0.1/LICENSE.txt` & `scMet-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scMet-1.0.1/README.rst` & `scMet-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `scMet-1.0.1/scMet/CVAEmodel.py` & `scMet-1.0.2/scMet/CVAEmodel.py`

 * *Files identical despite different names*

### Comparing `scMet-1.0.1/scMet/Dataloader.py` & `scMet-1.0.2/scMet/Dataloader.py`

 * *Files identical despite different names*

### Comparing `scMet-1.0.1/scMet/Deconvolution.py` & `scMet-1.0.2/scMet/Deconvolution.py`

 * *Files identical despite different names*

### Comparing `scMet-1.0.1/scMet/GenerateData.py` & `scMet-1.0.2/scMet/GenerateData.py`

 * *Files identical despite different names*

### Comparing `scMet-1.0.1/scMet/Main.py` & `scMet-1.0.2/scMet/Main.py`

 * *Files identical despite different names*

### Comparing `scMet-1.0.1/scMet/Simulation.py` & `scMet-1.0.2/scMet/Simulation.py`

 * *Files identical despite different names*

### Comparing `scMet-1.0.1/scMet/Std_choose.py` & `scMet-1.0.2/scMet/Std_choose.py`

 * *Files identical despite different names*

### Comparing `scMet-1.0.1/setup.py` & `scMet-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 
 def readme_file():
     with open("README.rst") as rf:
         return rf.read()
 
 setup(
     name='scMet',
-    version='1.0.1',
+    version='1.0.2',
     author='Gw yang',
     author_email='stu_gwyang@163.com',
     description='Fits bulk RNA-seq data using single-cell RNA-seq (scRNA-seq) data, enabling accurate estimation and analysis of gene expression profiles and metabolic flux balance',
     long_description='',
     url='https://github.com/your_username/your_package',
     packages=['scMet'],
     install_requires=[
         'scanpy',
         'pandas',
-        'combat == 0.2.1',
+        'combat==0.2.1',
         'numpy',
-        'warnings',
         'matplotlib',
         'sklearn',
         'tqdm',
         'scipy',
         'tensorflow',
-        'random',
         'anndata'
     ],
     python_requires='>=3.8',
 )
```

