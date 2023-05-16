# Comparing `tmp/pymiau-0.1.tar.gz` & `tmp/pymiau-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymiau-0.1.tar", last modified: Tue May 16 14:16:49 2023, max compression
+gzip compressed data, was "pymiau-0.2.tar", last modified: Tue May 16 14:38:46 2023, max compression
```

## Comparing `pymiau-0.1.tar` & `pymiau-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:16:49.051587 pymiau-0.1/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1134 2023-05-16 13:41:02.000000 pymiau-0.1/LICENSE
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1953 2023-05-16 14:16:49.051433 pymiau-0.1/PKG-INFO
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1518 2023-05-16 14:15:10.000000 pymiau-0.1/README.md
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:16:49.050082 pymiau-0.1/pymiau/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      500 2023-05-16 13:36:46.000000 pymiau-0.1/pymiau/__init__.py
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:16:49.050967 pymiau-0.1/pymiau.egg-info/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1953 2023-05-16 14:16:49.000000 pymiau-0.1/pymiau.egg-info/PKG-INFO
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      258 2023-05-16 14:16:49.000000 pymiau-0.1/pymiau.egg-info/SOURCES.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        1 2023-05-16 14:16:49.000000 pymiau-0.1/pymiau.egg-info/dependency_links.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       51 2023-05-16 14:16:49.000000 pymiau-0.1/pymiau.egg-info/entry_points.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       30 2023-05-16 14:16:49.000000 pymiau-0.1/pymiau.egg-info/requires.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        7 2023-05-16 14:16:49.000000 pymiau-0.1/pymiau.egg-info/top_level.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      131 2023-05-16 13:43:25.000000 pymiau-0.1/pyproject.toml
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       38 2023-05-16 14:16:49.051719 pymiau-0.1/setup.cfg
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2174 2023-05-16 14:15:22.000000 pymiau-0.1/setup.py
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:16:49.051086 pymiau-0.1/tests/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       19 2023-05-16 13:56:50.000000 pymiau-0.1/tests/test.py
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:38:46.632532 pymiau-0.2/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1134 2023-05-16 13:41:02.000000 pymiau-0.2/LICENSE
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2102 2023-05-16 14:38:46.632356 pymiau-0.2/PKG-INFO
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1667 2023-05-16 14:37:58.000000 pymiau-0.2/README.md
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:38:46.630803 pymiau-0.2/pymiau/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      500 2023-05-16 13:36:46.000000 pymiau-0.2/pymiau/__init__.py
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:38:46.631802 pymiau-0.2/pymiau.egg-info/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2102 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/PKG-INFO
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      258 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        1 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       51 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/entry_points.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       30 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/requires.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        7 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/top_level.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      131 2023-05-16 13:43:25.000000 pymiau-0.2/pyproject.toml
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       38 2023-05-16 14:38:46.632730 pymiau-0.2/setup.cfg
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2174 2023-05-16 14:38:42.000000 pymiau-0.2/setup.py
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:38:46.631942 pymiau-0.2/tests/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       19 2023-05-16 13:56:50.000000 pymiau-0.2/tests/test.py
```

### Comparing `pymiau-0.1/LICENSE` & `pymiau-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymiau-0.1/PKG-INFO` & `pymiau-0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: pymiau
-Version: 0.1
+Version: 0.2
 Summary: Make a Miau
 Home-page: https://pypi.org/project/pymiau
 Author: Fulan@ de Tal
 Author-email: fulano.de.tal@macondo.co
 License: MIT
 Keywords: Cats Dogs
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMiau
-## Use a short explanatory subtitle like, Make a Miau
+## Use a short explanatory subtitle like, Make a Miau and a Guau
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
 [![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/pymiau/)
 [![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/pymiau/)
 
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
-potential user do it.
+potential user do it!
+
+This is an example:
+
+<p align="center">
+<img src="https://images.pexels.com/photos/3777622/pexels-photo-3777622.jpeg" alt="Logo""/>
+</p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
```

### Comparing `pymiau-0.1/README.md` & `pymiau-0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # PyMiau
-## Use a short explanatory subtitle like, Make a Miau
+## Use a short explanatory subtitle like, Make a Miau and a Guau
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
 [![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/pymiau/)
 [![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/pymiau/)
 
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
-potential user do it.
+potential user do it!
+
+This is an example:
+
+<p align="center">
+<img src="https://images.pexels.com/photos/3777622/pexels-photo-3777622.jpeg" alt="Logo""/>
+</p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
```

### Comparing `pymiau-0.1/pymiau.egg-info/PKG-INFO` & `pymiau-0.2/pymiau.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: pymiau
-Version: 0.1
+Version: 0.2
 Summary: Make a Miau
 Home-page: https://pypi.org/project/pymiau
 Author: Fulan@ de Tal
 Author-email: fulano.de.tal@macondo.co
 License: MIT
 Keywords: Cats Dogs
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMiau
-## Use a short explanatory subtitle like, Make a Miau
+## Use a short explanatory subtitle like, Make a Miau and a Guau
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
 [![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/pymiau/)
 [![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/pymiau/)
 
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
-potential user do it.
+potential user do it!
+
+This is an example:
+
+<p align="center">
+<img src="https://images.pexels.com/photos/3777622/pexels-photo-3777622.jpeg" alt="Logo""/>
+</p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
```

### Comparing `pymiau-0.1/setup.py` & `pymiau-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.1',
+    version='0.2',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

