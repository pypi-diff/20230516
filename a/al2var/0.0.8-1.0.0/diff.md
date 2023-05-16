# Comparing `tmp/al2var-0.0.8.tar.gz` & `tmp/al2var-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/devel_al2var/forPypi/dist/.tmp-3p68z0mz/al2var-0.0.8.tar", last modified: Tue May 16 17:35:48 2023, max compression
+gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/devel_al2var/forPypi/dist/.tmp-dz8ub2y1/al2var-1.0.0.tar", last modified: Tue May 16 17:37:13 2023, max compression
```

## Comparing `al2var-0.0.8.tar` & `al2var-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-16 17:35:48.033613 al2var-0.0.8/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     1122 2022-10-08 19:49:45.000000 al2var-0.0.8/LICENSE
--rw-r--r--   0 hendrixj (1692218720) 1934156310       17 2022-10-10 23:15:11.000000 al2var-0.0.8/MANIFEST.in
--rw-r--r--   0 hendrixj (1692218720) 1934156310     7142 2023-05-16 17:35:48.033719 al2var-0.0.8/PKG-INFO
--rw-r--r--   0 hendrixj (1692218720) 1934156310     6617 2023-05-16 15:02:20.000000 al2var-0.0.8/README.md
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-16 17:35:48.033046 al2var-0.0.8/al2var.egg-info/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     7142 2023-05-16 17:35:48.000000 al2var-0.0.8/al2var.egg-info/PKG-INFO
--rw-r--r--   0 hendrixj (1692218720) 1934156310      179 2023-05-16 17:35:48.000000 al2var-0.0.8/al2var.egg-info/SOURCES.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-16 17:35:48.000000 al2var-0.0.8/al2var.egg-info/dependency_links.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-16 17:35:48.000000 al2var-0.0.8/al2var.egg-info/top_level.txt
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-16 17:35:48.033340 al2var-0.0.8/bin/
--rw-r--r--   0 hendrixj (1692218720) 1934156310    17784 2023-04-19 02:27:23.000000 al2var-0.0.8/bin/al2var
--rw-r--r--   0 hendrixj (1692218720) 1934156310       38 2023-05-16 17:35:48.034136 al2var-0.0.8/setup.cfg
--rw-r--r--   0 hendrixj (1692218720) 1934156310      824 2023-05-16 17:35:23.000000 al2var-0.0.8/setup.py
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-16 17:37:13.676036 al2var-1.0.0/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     1122 2022-10-08 19:49:45.000000 al2var-1.0.0/LICENSE
+-rw-r--r--   0 hendrixj (1692218720) 1934156310       17 2022-10-10 23:15:11.000000 al2var-1.0.0/MANIFEST.in
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     7140 2023-05-16 17:37:13.676136 al2var-1.0.0/PKG-INFO
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     6615 2023-05-16 17:36:40.000000 al2var-1.0.0/README.md
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-16 17:37:13.675480 al2var-1.0.0/al2var.egg-info/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     7140 2023-05-16 17:37:13.000000 al2var-1.0.0/al2var.egg-info/PKG-INFO
+-rw-r--r--   0 hendrixj (1692218720) 1934156310      179 2023-05-16 17:37:13.000000 al2var-1.0.0/al2var.egg-info/SOURCES.txt
+-rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-16 17:37:13.000000 al2var-1.0.0/al2var.egg-info/dependency_links.txt
+-rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-16 17:37:13.000000 al2var-1.0.0/al2var.egg-info/top_level.txt
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-16 17:37:13.675755 al2var-1.0.0/bin/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310    17784 2023-04-19 02:27:23.000000 al2var-1.0.0/bin/al2var
+-rw-r--r--   0 hendrixj (1692218720) 1934156310       38 2023-05-16 17:37:13.676603 al2var-1.0.0/setup.cfg
+-rw-r--r--   0 hendrixj (1692218720) 1934156310      824 2023-05-16 17:37:00.000000 al2var-1.0.0/setup.py
```

### Comparing `al2var-0.0.8/LICENSE` & `al2var-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `al2var-0.0.8/PKG-INFO` & `al2var-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: al2var
-Version: 0.0.8
+Version: 1.0.0
 Summary: Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence
 Home-page: https://github.com/jrhendrix/al2var
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 It is recomended by not required to install al2var in a conda environment. 
 
 Creating a possible conda environment for al2var:
 ```
 conda create -n al2var python=3.10.2 bcftools=1.14 samtools=1.14 bowtie2=2.5.1 minimap2=2.24
 ```
 
-al2var is available on [PyPI](https://pypi.org/project/roprokka/) and can be installed using pip.
+al2var is available on [PyPI](https://pypi.org/project/al2var/) and can be installed using pip.
 
 ```pip install al2var```
 
 OR clone from GitHub repository.
 
 ## Output
 al2var will create a directory to organize all of the generated output in various subdirectories.
```

### Comparing `al2var-0.0.8/README.md` & `al2var-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 It is recomended by not required to install al2var in a conda environment. 
 
 Creating a possible conda environment for al2var:
 ```
 conda create -n al2var python=3.10.2 bcftools=1.14 samtools=1.14 bowtie2=2.5.1 minimap2=2.24
 ```
 
-al2var is available on [PyPI](https://pypi.org/project/roprokka/) and can be installed using pip.
+al2var is available on [PyPI](https://pypi.org/project/al2var/) and can be installed using pip.
 
 ```pip install al2var```
 
 OR clone from GitHub repository.
 
 ## Output
 al2var will create a directory to organize all of the generated output in various subdirectories.
```

### Comparing `al2var-0.0.8/al2var.egg-info/PKG-INFO` & `al2var-1.0.0/al2var.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: al2var
-Version: 0.0.8
+Version: 1.0.0
 Summary: Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence
 Home-page: https://github.com/jrhendrix/al2var
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 It is recomended by not required to install al2var in a conda environment. 
 
 Creating a possible conda environment for al2var:
 ```
 conda create -n al2var python=3.10.2 bcftools=1.14 samtools=1.14 bowtie2=2.5.1 minimap2=2.24
 ```
 
-al2var is available on [PyPI](https://pypi.org/project/roprokka/) and can be installed using pip.
+al2var is available on [PyPI](https://pypi.org/project/al2var/) and can be installed using pip.
 
 ```pip install al2var```
 
 OR clone from GitHub repository.
 
 ## Output
 al2var will create a directory to organize all of the generated output in various subdirectories.
```

### Comparing `al2var-0.0.8/bin/al2var` & `al2var-1.0.0/bin/al2var`

 * *Files identical despite different names*

### Comparing `al2var-0.0.8/setup.py` & `al2var-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="al2var",
-    version="0.0.8",
+    version="1.0.0",
     author="Jo Hendrix",
     author_email="jrhendrix36@gmail.com",
     description="Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrhendrix/al2var",
     scripts=['bin/al2var'],
```

