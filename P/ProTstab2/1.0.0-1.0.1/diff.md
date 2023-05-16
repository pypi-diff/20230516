# Comparing `tmp/ProTstab2-1.0.0.tar.gz` & `tmp/ProTstab2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTstab2-1.0.0.tar", last modified: Tue May 16 06:29:17 2023, max compression
+gzip compressed data, was "ProTstab2-1.0.1.tar", last modified: Tue May 16 07:19:18 2023, max compression
```

## Comparing `ProTstab2-1.0.0.tar` & `ProTstab2-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 06:29:17.861730 ProTstab2-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-05-15 09:13:01.000000 ProTstab2-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2679 2023-05-16 06:29:17.860731 ProTstab2-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 06:29:17.854728 ProTstab2-1.0.0/ProTstab2/
--rw-rw-rw-   0        0        0     6087 2023-05-16 06:02:46.000000 ProTstab2-1.0.0/ProTstab2/__init__.py
--rw-rw-rw-   0        0        0     6192 2023-05-16 06:02:46.000000 ProTstab2-1.0.0/ProTstab2/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 06:29:17.859731 ProTstab2-1.0.0/ProTstab2.egg-info/
--rw-rw-rw-   0        0        0     2679 2023-05-16 06:29:17.000000 ProTstab2-1.0.0/ProTstab2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-16 06:29:17.000000 ProTstab2-1.0.0/ProTstab2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 06:29:17.000000 ProTstab2-1.0.0/ProTstab2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-16 06:29:17.000000 ProTstab2-1.0.0/ProTstab2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 06:29:17.000000 ProTstab2-1.0.0/ProTstab2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1958 2023-05-16 06:20:38.000000 ProTstab2-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 06:29:17.861730 ProTstab2-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1060 2023-05-16 06:29:16.000000 ProTstab2-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:19:18.199281 ProTstab2-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-15 09:13:01.000000 ProTstab2-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2679 2023-05-16 07:19:18.199281 ProTstab2-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 07:19:18.192783 ProTstab2-1.0.1/ProTstab2/
+-rw-rw-rw-   0        0        0     6087 2023-05-16 06:02:46.000000 ProTstab2-1.0.1/ProTstab2/__init__.py
+-rw-rw-rw-   0        0        0     6192 2023-05-16 06:02:46.000000 ProTstab2-1.0.1/ProTstab2/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:19:18.198282 ProTstab2-1.0.1/ProTstab2.egg-info/
+-rw-rw-rw-   0        0        0     2679 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 07:19:18.000000 ProTstab2-1.0.1/ProTstab2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2161 2023-05-16 06:21:35.000000 ProTstab2-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:19:18.199281 ProTstab2-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-05-16 07:18:57.000000 ProTstab2-1.0.1/setup.py
```

### Comparing `ProTstab2-1.0.0/LICENSE` & `ProTstab2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTstab2-1.0.0/PKG-INFO` & `ProTstab2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTstab2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Protein prediction package
 Home-page: http://8.133.174.28:8989/DeepTP/
 Author: Jianjun Zhao
 Author-email: 20204227057@stu.suda.edu.cn
 License: MIT
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `ProTstab2-1.0.0/ProTstab2/__init__.py` & `ProTstab2-1.0.1/ProTstab2/__init__.py`

 * *Files identical despite different names*

### Comparing `ProTstab2-1.0.0/ProTstab2/utils.py` & `ProTstab2-1.0.1/ProTstab2/utils.py`

 * *Files identical despite different names*

### Comparing `ProTstab2-1.0.0/ProTstab2.egg-info/PKG-INFO` & `ProTstab2-1.0.1/ProTstab2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTstab2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Protein prediction package
 Home-page: http://8.133.174.28:8989/DeepTP/
 Author: Jianjun Zhao
 Author-email: 20204227057@stu.suda.edu.cn
 License: MIT
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `ProTstab2-1.0.0/setup.py` & `ProTstab2-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 
 from distutils.core import setup
 
 from setuptools import find_packages
 
-with open("README_EN.md", "r", encoding='utf-8') as f:
+with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ProTstab2',  # 包名
-    version='1.0.0',  # 版本号
+    version='1.0.1',  # 版本号
     description='Protein prediction package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Jianjun Zhao',
     author_email='20204227057@stu.suda.edu.cn',
     url='http://8.133.174.28:8989/DeepTP/',
     install_requires=[
```

