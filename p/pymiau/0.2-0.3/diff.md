# Comparing `tmp/pymiau-0.2.tar.gz` & `tmp/pymiau-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymiau-0.2.tar", last modified: Tue May 16 14:38:46 2023, max compression
+gzip compressed data, was "pymiau-0.3.tar", last modified: Tue May 16 14:49:16 2023, max compression
```

## Comparing `pymiau-0.2.tar` & `pymiau-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:38:46.632532 pymiau-0.2/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1134 2023-05-16 13:41:02.000000 pymiau-0.2/LICENSE
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2102 2023-05-16 14:38:46.632356 pymiau-0.2/PKG-INFO
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1667 2023-05-16 14:37:58.000000 pymiau-0.2/README.md
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:38:46.630803 pymiau-0.2/pymiau/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      500 2023-05-16 13:36:46.000000 pymiau-0.2/pymiau/__init__.py
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:38:46.631802 pymiau-0.2/pymiau.egg-info/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2102 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/PKG-INFO
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      258 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/SOURCES.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        1 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/dependency_links.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       51 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/entry_points.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       30 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/requires.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        7 2023-05-16 14:38:46.000000 pymiau-0.2/pymiau.egg-info/top_level.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      131 2023-05-16 13:43:25.000000 pymiau-0.2/pyproject.toml
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       38 2023-05-16 14:38:46.632730 pymiau-0.2/setup.cfg
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2174 2023-05-16 14:38:42.000000 pymiau-0.2/setup.py
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:38:46.631942 pymiau-0.2/tests/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       19 2023-05-16 13:56:50.000000 pymiau-0.2/tests/test.py
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:49:16.785441 pymiau-0.3/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1134 2023-05-16 13:41:02.000000 pymiau-0.3/LICENSE
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2155 2023-05-16 14:49:16.785164 pymiau-0.3/PKG-INFO
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1720 2023-05-16 14:47:43.000000 pymiau-0.3/README.md
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:49:16.783686 pymiau-0.3/pymiau/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      500 2023-05-16 13:36:46.000000 pymiau-0.3/pymiau/__init__.py
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:49:16.784019 pymiau-0.3/pymiau/data/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)    27919 2023-05-16 14:40:18.000000 pymiau-0.3/pymiau/data/miau.jpeg
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-05-16 14:49:16.784978 pymiau-0.3/pymiau.egg-info/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2155 2023-05-16 14:49:16.000000 pymiau-0.3/pymiau.egg-info/PKG-INFO
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      268 2023-05-16 14:49:16.000000 pymiau-0.3/pymiau.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        1 2023-05-16 14:49:16.000000 pymiau-0.3/pymiau.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       51 2023-05-16 14:49:16.000000 pymiau-0.3/pymiau.egg-info/entry_points.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       30 2023-05-16 14:49:16.000000 pymiau-0.3/pymiau.egg-info/requires.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        7 2023-05-16 14:49:16.000000 pymiau-0.3/pymiau.egg-info/top_level.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      131 2023-05-16 13:43:25.000000 pymiau-0.3/pyproject.toml
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       38 2023-05-16 14:49:16.785485 pymiau-0.3/setup.cfg
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2174 2023-05-16 14:40:28.000000 pymiau-0.3/setup.py
```

### Comparing `pymiau-0.2/LICENSE` & `pymiau-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymiau-0.2/PKG-INFO` & `pymiau-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymiau
-Version: 0.2
+Version: 0.3
 Summary: Make a Miau
 Home-page: https://pypi.org/project/pymiau
 Author: Fulan@ de Tal
 Author-email: fulano.de.tal@macondo.co
 License: MIT
 Keywords: Cats Dogs
 Platform: UNKNOWN
@@ -24,15 +24,15 @@
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
 <p align="center">
-<img src="https://images.pexels.com/photos/3777622/pexels-photo-3777622.jpeg" alt="Logo""/>
+<img src="https://github.com/seap-udea/murray-dermott-action/blob/main/tutorials/PythonPackages/pymiau-dist/pymiau/data/miau.jpeg" alt="Logo""/>
 </p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
```

### Comparing `pymiau-0.2/README.md` & `pymiau-0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
 <p align="center">
-<img src="https://images.pexels.com/photos/3777622/pexels-photo-3777622.jpeg" alt="Logo""/>
+<img src="https://github.com/seap-udea/murray-dermott-action/blob/main/tutorials/PythonPackages/pymiau-dist/pymiau/data/miau.jpeg" alt="Logo""/>
 </p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
```

### Comparing `pymiau-0.2/pymiau.egg-info/PKG-INFO` & `pymiau-0.3/pymiau.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymiau
-Version: 0.2
+Version: 0.3
 Summary: Make a Miau
 Home-page: https://pypi.org/project/pymiau
 Author: Fulan@ de Tal
 Author-email: fulano.de.tal@macondo.co
 License: MIT
 Keywords: Cats Dogs
 Platform: UNKNOWN
@@ -24,15 +24,15 @@
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
 <p align="center">
-<img src="https://images.pexels.com/photos/3777622/pexels-photo-3777622.jpeg" alt="Logo""/>
+<img src="https://github.com/seap-udea/murray-dermott-action/blob/main/tutorials/PythonPackages/pymiau-dist/pymiau/data/miau.jpeg" alt="Logo""/>
 </p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
```

### Comparing `pymiau-0.2/setup.py` & `pymiau-0.3/setup.py`

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
-    version='0.2',
+    version='0.3',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

