# Comparing `tmp/CustomerProfile-0.1.0.tar.gz` & `tmp/CustomerProfile-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CustomerProfile-0.1.0.tar", last modified: Tue May 16 19:31:25 2023, max compression
+gzip compressed data, was "dist\CustomerProfile-0.1.1.tar", last modified: Tue May 16 19:42:33 2023, max compression
```

## Comparing `CustomerProfile-0.1.0.tar` & `CustomerProfile-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:31:25.699435 CustomerProfile-0.1.0/
--rw-rw-rw-   0        0        0      178 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3763 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/CONTRIBUTING.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 19:31:25.581037 CustomerProfile-0.1.0/CustomerProfile/
--rw-rw-rw-   0        0        0    11331 2023-05-16 19:19:21.000000 CustomerProfile-0.1.0/CustomerProfile/CustomerProfile.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:31:25.627112 CustomerProfile-0.1.0/CustomerProfile/Data/
--rw-rw-rw-   0        0        0        0 2023-05-16 18:57:56.000000 CustomerProfile-0.1.0/CustomerProfile/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:31:25.641318 CustomerProfile-0.1.0/CustomerProfile/Preprocessing/
--rw-rw-rw-   0        0        0       94 2023-05-16 18:58:34.000000 CustomerProfile-0.1.0/CustomerProfile/Preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2121 2023-05-16 19:27:20.000000 CustomerProfile-0.1.0/CustomerProfile/Preprocessing/outlier.py
--rw-rw-rw-   0        0        0     7653 2023-05-16 19:26:44.000000 CustomerProfile-0.1.0/CustomerProfile/Preprocessing/scaler.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:31:25.652478 CustomerProfile-0.1.0/CustomerProfile/Report/
--rw-rw-rw-   0        0        0        0 2023-05-16 18:58:03.000000 CustomerProfile-0.1.0/CustomerProfile/Report/__init__.py
--rw-rw-rw-   0        0        0      246 2023-05-16 18:56:52.000000 CustomerProfile-0.1.0/CustomerProfile/__init__.py
--rw-rw-rw-   0        0        0     6385 2023-05-16 19:22:14.000000 CustomerProfile-0.1.0/CustomerProfile/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:31:25.624043 CustomerProfile-0.1.0/CustomerProfile.egg-info/
--rw-rw-rw-   0        0        0     1885 2023-05-16 19:31:25.000000 CustomerProfile-0.1.0/CustomerProfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      728 2023-05-16 19:31:25.000000 CustomerProfile-0.1.0/CustomerProfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:31:25.000000 CustomerProfile-0.1.0/CustomerProfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 18:55:58.000000 CustomerProfile-0.1.0/CustomerProfile.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-05-16 19:31:25.000000 CustomerProfile-0.1.0/CustomerProfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1095 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1885 2023-05-16 19:31:25.700435 CustomerProfile-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1008 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 19:31:25.697437 CustomerProfile-0.1.0/docs/
--rw-rw-rw-   0        0        0      636 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     5050 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      332 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1249 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      813 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       92 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/docs/usage.rst
--rw-rw-rw-   0        0        0      410 2023-05-16 19:31:25.703506 CustomerProfile-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-16 16:46:24.000000 CustomerProfile-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:42:33.442983 CustomerProfile-0.1.1/
+-rw-rw-rw-   0        0        0      178 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3763 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/CONTRIBUTING.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 19:42:33.279947 CustomerProfile-0.1.1/CustomerProfile/
+-rw-rw-rw-   0        0        0    11331 2023-05-16 19:19:21.000000 CustomerProfile-0.1.1/CustomerProfile/CustomerProfile.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:42:33.345702 CustomerProfile-0.1.1/CustomerProfile/Data/
+-rw-rw-rw-   0        0        0        0 2023-05-16 18:57:56.000000 CustomerProfile-0.1.1/CustomerProfile/Data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:42:33.359705 CustomerProfile-0.1.1/CustomerProfile/Preprocessing/
+-rw-rw-rw-   0        0        0       94 2023-05-16 18:58:34.000000 CustomerProfile-0.1.1/CustomerProfile/Preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2121 2023-05-16 19:27:20.000000 CustomerProfile-0.1.1/CustomerProfile/Preprocessing/outlier.py
+-rw-rw-rw-   0        0        0     7653 2023-05-16 19:26:44.000000 CustomerProfile-0.1.1/CustomerProfile/Preprocessing/scaler.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:42:33.370748 CustomerProfile-0.1.1/CustomerProfile/Report/
+-rw-rw-rw-   0        0        0        0 2023-05-16 18:58:03.000000 CustomerProfile-0.1.1/CustomerProfile/Report/__init__.py
+-rw-rw-rw-   0        0        0      246 2023-05-16 18:56:52.000000 CustomerProfile-0.1.1/CustomerProfile/__init__.py
+-rw-rw-rw-   0        0        0     6385 2023-05-16 19:22:14.000000 CustomerProfile-0.1.1/CustomerProfile/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:42:33.342793 CustomerProfile-0.1.1/CustomerProfile.egg-info/
+-rw-rw-rw-   0        0        0     1885 2023-05-16 19:42:33.000000 CustomerProfile-0.1.1/CustomerProfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      766 2023-05-16 19:42:33.000000 CustomerProfile-0.1.1/CustomerProfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 19:42:33.000000 CustomerProfile-0.1.1/CustomerProfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 18:55:58.000000 CustomerProfile-0.1.1/CustomerProfile.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2023-05-16 19:42:33.000000 CustomerProfile-0.1.1/CustomerProfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 19:42:33.000000 CustomerProfile-0.1.1/CustomerProfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1095 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1885 2023-05-16 19:42:33.442983 CustomerProfile-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1008 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 19:42:33.440983 CustomerProfile-0.1.1/docs/
+-rw-rw-rw-   0        0        0      636 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     5050 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      332 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1249 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      813 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       92 2023-05-16 16:46:24.000000 CustomerProfile-0.1.1/docs/usage.rst
+-rw-rw-rw-   0        0        0      410 2023-05-16 19:42:33.454033 CustomerProfile-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-05-16 19:42:29.000000 CustomerProfile-0.1.1/setup.py
```

### Comparing `CustomerProfile-0.1.0/CONTRIBUTING.rst` & `CustomerProfile-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/CustomerProfile/CustomerProfile.py` & `CustomerProfile-0.1.1/CustomerProfile/CustomerProfile.py`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/CustomerProfile/Preprocessing/outlier.py` & `CustomerProfile-0.1.1/CustomerProfile/Preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/CustomerProfile/Preprocessing/scaler.py` & `CustomerProfile-0.1.1/CustomerProfile/Preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/CustomerProfile/utils.py` & `CustomerProfile-0.1.1/CustomerProfile/utils.py`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/CustomerProfile.egg-info/PKG-INFO` & `CustomerProfile-0.1.1/CustomerProfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomerProfile
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use package for customer profile creation in Python.
 Home-page: https://github.com/HrayrMuradyan/CustomerProfile
 Author: Hrayr Muradyan
 Author-email: hrayrmuradyan20@gmail.com
 License: MIT license
 Keywords: CustomerProfile
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `CustomerProfile-0.1.0/CustomerProfile.egg-info/SOURCES.txt` & `CustomerProfile-0.1.1/CustomerProfile.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 CustomerProfile/CustomerProfile.py
 CustomerProfile/__init__.py
 CustomerProfile/utils.py
 CustomerProfile.egg-info/PKG-INFO
 CustomerProfile.egg-info/SOURCES.txt
 CustomerProfile.egg-info/dependency_links.txt
 CustomerProfile.egg-info/not-zip-safe
+CustomerProfile.egg-info/requires.txt
 CustomerProfile.egg-info/top_level.txt
 CustomerProfile/Data/__init__.py
 CustomerProfile/Preprocessing/__init__.py
 CustomerProfile/Preprocessing/outlier.py
 CustomerProfile/Preprocessing/scaler.py
 CustomerProfile/Report/__init__.py
 docs/Makefile
```

### Comparing `CustomerProfile-0.1.0/LICENSE` & `CustomerProfile-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/PKG-INFO` & `CustomerProfile-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomerProfile
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use package for customer profile creation in Python.
 Home-page: https://github.com/HrayrMuradyan/CustomerProfile
 Author: Hrayr Muradyan
 Author-email: hrayrmuradyan20@gmail.com
 License: MIT license
 Keywords: CustomerProfile
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `CustomerProfile-0.1.0/README.rst` & `CustomerProfile-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/docs/Makefile` & `CustomerProfile-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/docs/conf.py` & `CustomerProfile-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/docs/installation.rst` & `CustomerProfile-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/docs/make.bat` & `CustomerProfile-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `CustomerProfile-0.1.0/setup.py` & `CustomerProfile-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,39 +6,34 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = [ ]
-
-test_requirements = [ ]
-
 setup(
     author="Hrayr Muradyan",
     author_email='hrayrmuradyan20@gmail.com',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
+    install_requires=['pandas', 'numpy', 'scikit-learn', 'matplotlib'],
     description="An easy-to-use package for customer profile creation in Python.",
-    install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='CustomerProfile',
     name='CustomerProfile',
     packages=find_packages(include=['CustomerProfile', 'CustomerProfile.*']),
     test_suite='tests',
-    tests_require=test_requirements,
     url='https://github.com/HrayrMuradyan/CustomerProfile',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

