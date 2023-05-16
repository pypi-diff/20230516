# Comparing `tmp/isoCycle-0.0.2.tar.gz` & `tmp/isoCycle-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\isoCycle-0.0.2.tar", last modified: Tue May 16 02:36:43 2023, max compression
+gzip compressed data, was "dist\isoCycle-0.0.3.tar", last modified: Tue May 16 02:42:11 2023, max compression
```

## Comparing `isoCycle-0.0.2.tar` & `isoCycle-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 02:36:43.000000 isoCycle-0.0.2/
--rw-rw-rw-   0        0        0      546 2023-05-16 02:36:43.000000 isoCycle-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2059 2023-05-15 17:32:06.000000 isoCycle-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 02:36:43.000000 isoCycle-0.0.2/isoCycle/
--rw-rw-rw-   0        0        0       43 2023-05-16 01:12:23.000000 isoCycle-0.0.2/isoCycle/__init__.py
--rw-rw-rw-   0        0        0     9147 2023-05-16 01:07:24.000000 isoCycle-0.0.2/isoCycle/decoder.py
--rw-rw-rw-   0        0        0     2842 2023-05-15 19:09:11.000000 isoCycle-0.0.2/isoCycle/spike.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:36:43.000000 isoCycle-0.0.2/isoCycle.egg-info/
--rw-rw-rw-   0        0        0      546 2023-05-16 02:36:43.000000 isoCycle-0.0.2/isoCycle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-16 02:36:43.000000 isoCycle-0.0.2/isoCycle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 02:36:43.000000 isoCycle-0.0.2/isoCycle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-16 02:36:43.000000 isoCycle-0.0.2/isoCycle.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 02:36:43.000000 isoCycle-0.0.2/isoCycle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 02:36:43.000000 isoCycle-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-05-16 02:36:33.000000 isoCycle-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:42:11.000000 isoCycle-0.0.3/
+-rw-rw-rw-   0        0        0      546 2023-05-16 02:42:11.000000 isoCycle-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2059 2023-05-15 17:32:06.000000 isoCycle-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 02:42:11.000000 isoCycle-0.0.3/isoCycle/
+-rw-rw-rw-   0        0        0       43 2023-05-16 01:12:23.000000 isoCycle-0.0.3/isoCycle/__init__.py
+-rw-rw-rw-   0        0        0     9147 2023-05-16 01:07:24.000000 isoCycle-0.0.3/isoCycle/decoder.py
+-rw-rw-rw-   0        0        0     2842 2023-05-15 19:09:11.000000 isoCycle-0.0.3/isoCycle/spike.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:42:11.000000 isoCycle-0.0.3/isoCycle.egg-info/
+-rw-rw-rw-   0        0        0      546 2023-05-16 02:42:11.000000 isoCycle-0.0.3/isoCycle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-16 02:42:11.000000 isoCycle-0.0.3/isoCycle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 02:42:11.000000 isoCycle-0.0.3/isoCycle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-16 02:42:11.000000 isoCycle-0.0.3/isoCycle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 02:42:11.000000 isoCycle-0.0.3/isoCycle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 02:42:11.000000 isoCycle-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-05-16 02:42:00.000000 isoCycle-0.0.3/setup.py
```

### Comparing `isoCycle-0.0.2/PKG-INFO` & `isoCycle-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: isoCycle
-Version: 0.0.2
+Version: 0.0.3
 Summary: isolating single cycles in neuronal spiking
 Home-page: https://github.com/esiabri/isoCycle
 Author: Ehsan Sabri
 Author-email: ehsan.sabri@gmail.com
 License: CC-BY-NC-SA-4.0
 Download-URL: https://github.com/esiabri/isoCycle/archive/refs/tags/0.0.1.tar.gz
 Description: UNKNOWN
```

### Comparing `isoCycle-0.0.2/README.md` & `isoCycle-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `isoCycle-0.0.2/isoCycle/decoder.py` & `isoCycle-0.0.3/isoCycle/decoder.py`

 * *Files identical despite different names*

### Comparing `isoCycle-0.0.2/isoCycle/spike.py` & `isoCycle-0.0.3/isoCycle/spike.py`

 * *Files identical despite different names*

### Comparing `isoCycle-0.0.2/isoCycle.egg-info/PKG-INFO` & `isoCycle-0.0.3/isoCycle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: isoCycle
-Version: 0.0.2
+Version: 0.0.3
 Summary: isolating single cycles in neuronal spiking
 Home-page: https://github.com/esiabri/isoCycle
 Author: Ehsan Sabri
 Author-email: ehsan.sabri@gmail.com
 License: CC-BY-NC-SA-4.0
 Download-URL: https://github.com/esiabri/isoCycle/archive/refs/tags/0.0.1.tar.gz
 Description: UNKNOWN
```

### Comparing `isoCycle-0.0.2/setup.py` & `isoCycle-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
   name = 'isoCycle',         
   packages = ['isoCycle'],   
-  version = '0.0.2',      
+  version = '0.0.3',      
   license='CC-BY-NC-SA-4.0',        
   description = 'isolating single cycles in neuronal spiking',   
   author = 'Ehsan Sabri',                   
   author_email = 'ehsan.sabri@gmail.com',      
   url = 'https://github.com/esiabri/isoCycle',  
   download_url = 'https://github.com/esiabri/isoCycle/archive/refs/tags/0.0.1.tar.gz',   
   keywords = ['Neuroscience', 'Oscillation', 'Cycle'],
```

