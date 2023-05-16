# Comparing `tmp/azurify-0.5.tar.gz` & `tmp/azurify-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurify-0.5.tar", last modified: Fri May  5 08:30:40 2023, max compression
+gzip compressed data, was "azurify-0.6.tar", last modified: Tue May 16 11:04:55 2023, max compression
```

## Comparing `azurify-0.5.tar` & `azurify-0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 deniz      (501) admin       (80)        0 2023-05-05 08:30:40.304564 azurify-0.5/
--rw-r--r--   0 deniz      (501) admin       (80)     1067 2023-05-03 10:36:25.000000 azurify-0.5/LICENSE
--rw-r--r--   0 deniz      (501) admin       (80)     3080 2023-05-05 08:30:40.304261 azurify-0.5/PKG-INFO
-drwxr-xr-x   0 deniz      (501) admin       (80)        0 2023-05-05 08:30:40.303067 azurify-0.5/azurify/
--rw-r--r--   0 deniz      (501) admin       (80)      108 2023-05-04 15:35:26.000000 azurify-0.5/azurify/__init__.py
--rw-r--r--   0 deniz      (501) admin       (80)     1627 2023-05-04 14:36:19.000000 azurify-0.5/azurify/azconverter.py
--rw-r--r--   0 deniz      (501) admin       (80)     3370 2023-05-04 10:21:42.000000 azurify-0.5/azurify/azkeyvault.py
--rw-r--r--   0 deniz      (501) admin       (80)     3556 2023-05-03 12:12:17.000000 azurify-0.5/azurify/azsecrets.py
--rw-r--r--   0 deniz      (501) admin       (80)     3014 2023-05-04 10:22:29.000000 azurify-0.5/azurify/azstorage.py
--rw-r--r--   0 deniz      (501) admin       (80)      547 2023-05-03 10:29:22.000000 azurify-0.5/azurify/test_azconverter.py
--rw-r--r--   0 deniz      (501) admin       (80)     1393 2023-04-27 06:26:58.000000 azurify-0.5/azurify/test_azkeyvault.py
--rw-r--r--   0 deniz      (501) admin       (80)     3679 2023-05-03 11:03:20.000000 azurify-0.5/azurify/test_azsecrets.py
--rw-r--r--   0 deniz      (501) admin       (80)        0 2023-04-25 11:33:39.000000 azurify-0.5/azurify/test_azstorage.py
-drwxr-xr-x   0 deniz      (501) admin       (80)        0 2023-05-05 08:30:40.304043 azurify-0.5/azurify.egg-info/
--rw-r--r--   0 deniz      (501) admin       (80)     3080 2023-05-05 08:30:40.000000 azurify-0.5/azurify.egg-info/PKG-INFO
--rw-r--r--   0 deniz      (501) admin       (80)      414 2023-05-05 08:30:40.000000 azurify-0.5/azurify.egg-info/SOURCES.txt
--rw-r--r--   0 deniz      (501) admin       (80)        1 2023-05-05 08:30:40.000000 azurify-0.5/azurify.egg-info/dependency_links.txt
--rw-r--r--   0 deniz      (501) admin       (80)        1 2023-05-04 14:43:06.000000 azurify-0.5/azurify.egg-info/not-zip-safe
--rw-r--r--   0 deniz      (501) admin       (80)      133 2023-05-05 08:30:40.000000 azurify-0.5/azurify.egg-info/requires.txt
--rw-r--r--   0 deniz      (501) admin       (80)        8 2023-05-05 08:30:40.000000 azurify-0.5/azurify.egg-info/top_level.txt
--rw-r--r--   0 deniz      (501) admin       (80)       38 2023-05-05 08:30:40.304654 azurify-0.5/setup.cfg
--rw-r--r--   0 deniz      (501) admin       (80)     1051 2023-05-05 08:30:20.000000 azurify-0.5/setup.py
+drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-16 11:04:55.777759 azurify-0.6/
+-rw-r--r--   0 deniz      (501) staff       (20)     1067 2023-05-15 16:05:12.000000 azurify-0.6/LICENSE
+-rw-r--r--   0 deniz      (501) staff       (20)     3026 2023-05-16 11:04:55.777077 azurify-0.6/PKG-INFO
+drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-16 11:04:55.764272 azurify-0.6/azurify/
+-rw-r--r--   0 deniz      (501) staff       (20)      108 2023-05-15 16:05:12.000000 azurify-0.6/azurify/__init__.py
+-rw-r--r--   0 deniz      (501) staff       (20)     1627 2023-05-15 16:05:12.000000 azurify-0.6/azurify/azconverter.py
+-rw-r--r--   0 deniz      (501) staff       (20)     4511 2023-05-16 10:29:00.000000 azurify-0.6/azurify/azkeyvault.py
+-rw-r--r--   0 deniz      (501) staff       (20)     3556 2023-05-15 16:05:12.000000 azurify-0.6/azurify/azsecrets.py
+-rw-r--r--   0 deniz      (501) staff       (20)     3014 2023-05-15 16:05:12.000000 azurify-0.6/azurify/azstorage.py
+-rw-r--r--   0 deniz      (501) staff       (20)      547 2023-05-15 16:05:12.000000 azurify-0.6/azurify/test_azconverter.py
+-rw-r--r--   0 deniz      (501) staff       (20)     1393 2023-05-15 16:05:12.000000 azurify-0.6/azurify/test_azkeyvault.py
+-rw-r--r--   0 deniz      (501) staff       (20)     3679 2023-05-15 16:05:12.000000 azurify-0.6/azurify/test_azsecrets.py
+-rw-r--r--   0 deniz      (501) staff       (20)        0 2023-05-15 16:05:12.000000 azurify-0.6/azurify/test_azstorage.py
+drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-16 11:04:55.773603 azurify-0.6/azurify.egg-info/
+-rw-r--r--   0 deniz      (501) staff       (20)     3026 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/PKG-INFO
+-rw-r--r--   0 deniz      (501) staff       (20)      414 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/SOURCES.txt
+-rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/dependency_links.txt
+-rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-16 09:30:41.000000 azurify-0.6/azurify.egg-info/not-zip-safe
+-rw-r--r--   0 deniz      (501) staff       (20)      133 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/requires.txt
+-rw-r--r--   0 deniz      (501) staff       (20)        8 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/top_level.txt
+-rw-r--r--   0 deniz      (501) staff       (20)       38 2023-05-16 11:04:55.778591 azurify-0.6/setup.cfg
+-rw-r--r--   0 deniz      (501) staff       (20)      997 2023-05-16 10:49:32.000000 azurify-0.6/setup.py
```

### Comparing `azurify-0.5/LICENSE` & `azurify-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `azurify-0.5/PKG-INFO` & `azurify-0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: azurify
-Version: 0.5
+Version: 0.6
 Summary: Access to Azure Storage/Secrets/Keyvault for Shopify Apps built with Python.
 Home-page: https://github.com/zinyosrim/azurify
 Author: Zin Yosrim
 Author-email: zinyosrim@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Azure resource access library for Shopify Apps
 The motivation for this library arose out of a data analysis project for a Shopify 
@@ -105,18 +103,17 @@
 ```
     cd testazurify
     python3 -m venv .venv
     source .venv/bin/activate
     pip install -e ../azurify
 
 
-### Upload to repository
+### Upload to test repository
     cd ../azurify
     pip install twine
     twine check dist/*
     twine upload -r testpypi dist/*
 
-    twine upload -r dist/*
+### Upload to Pypi
+    twine upload dist/*
 
 [src]: https://github.com/zinyosrim/azurify
-
-
```

### Comparing `azurify-0.5/azurify/azconverter.py` & `azurify-0.6/azurify/azconverter.py`

 * *Files identical despite different names*

### Comparing `azurify-0.5/azurify/azsecrets.py` & `azurify-0.6/azurify/azsecrets.py`

 * *Files identical despite different names*

### Comparing `azurify-0.5/azurify/azstorage.py` & `azurify-0.6/azurify/azstorage.py`

 * *Files identical despite different names*

### Comparing `azurify-0.5/azurify/test_azconverter.py` & `azurify-0.6/azurify/test_azconverter.py`

 * *Files identical despite different names*

### Comparing `azurify-0.5/azurify/test_azkeyvault.py` & `azurify-0.6/azurify/test_azkeyvault.py`

 * *Files identical despite different names*

### Comparing `azurify-0.5/azurify/test_azsecrets.py` & `azurify-0.6/azurify/test_azsecrets.py`

 * *Files identical despite different names*

### Comparing `azurify-0.5/azurify.egg-info/PKG-INFO` & `azurify-0.6/azurify.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: azurify
-Version: 0.5
+Version: 0.6
 Summary: Access to Azure Storage/Secrets/Keyvault for Shopify Apps built with Python.
 Home-page: https://github.com/zinyosrim/azurify
 Author: Zin Yosrim
 Author-email: zinyosrim@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Azure resource access library for Shopify Apps
 The motivation for this library arose out of a data analysis project for a Shopify 
@@ -105,18 +103,17 @@
 ```
     cd testazurify
     python3 -m venv .venv
     source .venv/bin/activate
     pip install -e ../azurify
 
 
-### Upload to repository
+### Upload to test repository
     cd ../azurify
     pip install twine
     twine check dist/*
     twine upload -r testpypi dist/*
 
-    twine upload -r dist/*
+### Upload to Pypi
+    twine upload dist/*
 
 [src]: https://github.com/zinyosrim/azurify
-
-
```

### Comparing `azurify-0.5/setup.py` & `azurify-0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import find_packages, setup
 
 with open("Readme.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="azurify",
-    version="0.5",
+    version="0.6",
     description="Access to Azure Storage/Secrets/Keyvault for Shopify Apps built with Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zinyosrim/azurify",
     author="Zin Yosrim",
     author_email="zinyosrim@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
-        "Development Status :: 5 - Production/Stable",
     ],
     packages=find_packages(),
     install_requires=[
         "pandas",
         "StrEnum",
         "azure-identity",
         "azure-keyvault-secrets",
```

