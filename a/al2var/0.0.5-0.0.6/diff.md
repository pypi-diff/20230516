# Comparing `tmp/al2var-0.0.5.tar.gz` & `tmp/al2var-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/devel_al2var/forPypi/dist/.tmp-77boqn9g/al2var-0.0.5.tar", last modified: Wed Apr 19 03:01:27 2023, max compression
+gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/devel_al2var/forPypi/dist/.tmp-c9d70512/al2var-0.0.6.tar", last modified: Mon May 15 23:30:16 2023, max compression
```

## Comparing `al2var-0.0.5.tar` & `al2var-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-04-19 03:01:27.250529 al2var-0.0.5/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     1122 2022-10-08 19:49:45.000000 al2var-0.0.5/LICENSE
--rw-r--r--   0 hendrixj (1692218720) 1934156310       17 2022-10-10 23:15:11.000000 al2var-0.0.5/MANIFEST.in
--rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-04-19 03:01:27.250687 al2var-0.0.5/PKG-INFO
--rw-r--r--   0 hendrixj (1692218720) 1934156310     6499 2023-04-19 02:14:41.000000 al2var-0.0.5/README.md
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-04-19 03:01:27.248735 al2var-0.0.5/al2var.egg-info/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-04-19 03:01:27.000000 al2var-0.0.5/al2var.egg-info/PKG-INFO
--rw-r--r--   0 hendrixj (1692218720) 1934156310      208 2023-04-19 03:01:27.000000 al2var-0.0.5/al2var.egg-info/SOURCES.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-04-19 03:01:27.000000 al2var-0.0.5/al2var.egg-info/dependency_links.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310       23 2023-04-19 03:01:27.000000 al2var-0.0.5/al2var.egg-info/requires.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-04-19 03:01:27.000000 al2var-0.0.5/al2var.egg-info/top_level.txt
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-04-19 03:01:27.249437 al2var-0.0.5/bin/
--rw-r--r--   0 hendrixj (1692218720) 1934156310    17784 2023-04-19 02:27:23.000000 al2var-0.0.5/bin/al2var
--rw-r--r--   0 hendrixj (1692218720) 1934156310       38 2023-04-19 03:01:27.251324 al2var-0.0.5/setup.cfg
--rw-r--r--   0 hendrixj (1692218720) 1934156310      854 2023-04-19 03:01:03.000000 al2var-0.0.5/setup.py
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-15 23:30:16.918311 al2var-0.0.6/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     1122 2022-10-08 19:49:45.000000 al2var-0.0.6/LICENSE
+-rw-r--r--   0 hendrixj (1692218720) 1934156310       17 2022-10-10 23:15:11.000000 al2var-0.0.6/MANIFEST.in
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-05-15 23:30:16.918516 al2var-0.0.6/PKG-INFO
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     6499 2023-04-19 02:14:41.000000 al2var-0.0.6/README.md
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-15 23:30:16.916538 al2var-0.0.6/al2var.egg-info/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-05-15 23:30:16.000000 al2var-0.0.6/al2var.egg-info/PKG-INFO
+-rw-r--r--   0 hendrixj (1692218720) 1934156310      179 2023-05-15 23:30:16.000000 al2var-0.0.6/al2var.egg-info/SOURCES.txt
+-rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-15 23:30:16.000000 al2var-0.0.6/al2var.egg-info/dependency_links.txt
+-rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-05-15 23:30:16.000000 al2var-0.0.6/al2var.egg-info/top_level.txt
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-05-15 23:30:16.917192 al2var-0.0.6/bin/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310    17784 2023-04-19 02:27:23.000000 al2var-0.0.6/bin/al2var
+-rw-r--r--   0 hendrixj (1692218720) 1934156310       38 2023-05-15 23:30:16.919144 al2var-0.0.6/setup.cfg
+-rw-r--r--   0 hendrixj (1692218720) 1934156310      824 2023-05-15 23:28:59.000000 al2var-0.0.6/setup.py
```

### Comparing `al2var-0.0.5/LICENSE` & `al2var-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `al2var-0.0.5/PKG-INFO` & `al2var-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: al2var
-Version: 0.0.5
+Version: 0.0.6
 Summary: Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence
 Home-page: https://github.com/jrhendrix/al2var
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `al2var-0.0.5/README.md` & `al2var-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `al2var-0.0.5/al2var.egg-info/PKG-INFO` & `al2var-0.0.6/al2var.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: al2var
-Version: 0.0.5
+Version: 0.0.6
 Summary: Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence
 Home-page: https://github.com/jrhendrix/al2var
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `al2var-0.0.5/bin/al2var` & `al2var-0.0.6/bin/al2var`

 * *Files identical despite different names*

### Comparing `al2var-0.0.5/setup.py` & `al2var-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="al2var",
-    version="0.0.5",
+    version="0.0.6",
     author="Jo Hendrix",
     author_email="jrhendrix36@gmail.com",
     description="Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrhendrix/al2var",
     scripts=['bin/al2var'],
     packages=setuptools.find_packages(),
     include_package_data=True,
-    install_requires=['xsamtools', 'bowtie', 'mappy'],
+    install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
 )
```

