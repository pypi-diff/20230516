# Comparing `tmp/slicpy-0.0.5.tar.gz` & `tmp/slicpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicpy-0.0.5.tar", last modified: Tue May 16 03:22:02 2023, max compression
+gzip compressed data, was "slicpy-0.0.6.tar", last modified: Tue May 16 03:23:49 2023, max compression
```

## Comparing `slicpy-0.0.5.tar` & `slicpy-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:22:02.631211 slicpy-0.0.5/
--rw-r--r--   0 teddyoweh   (501) staff       (20)     6002 2023-05-16 03:22:02.631284 slicpy-0.0.5/PKG-INFO
--rw-r--r--   0 teddyoweh   (501) staff       (20)     5618 2023-05-16 03:09:14.000000 slicpy-0.0.5/README.md
--rw-r--r--   0 teddyoweh   (501) staff       (20)      107 2023-05-16 03:22:02.631700 slicpy-0.0.5/setup.cfg
--rw-r--r--   0 teddyoweh   (501) staff       (20)     1002 2023-05-16 03:21:23.000000 slicpy-0.0.5/setup.py
-drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:22:02.630033 slicpy-0.0.5/slicpy/
--rw-r--r--   0 teddyoweh   (501) staff       (20)     1373 2023-05-02 15:55:53.000000 slicpy-0.0.5/slicpy/Console.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)      650 2023-05-15 22:56:23.000000 slicpy-0.0.5/slicpy/HashMap.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     1009 2023-05-15 23:17:16.000000 slicpy-0.0.5/slicpy/NetworkTrafficMap.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)      700 2023-05-15 22:55:30.000000 slicpy-0.0.5/slicpy/Rate.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     8352 2023-05-15 22:56:54.000000 slicpy-0.0.5/slicpy/Slic.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)      154 2023-05-16 03:21:10.000000 slicpy-0.0.5/slicpy/__init__.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     3015 2023-05-02 11:02:36.000000 slicpy-0.0.5/slicpy/decorators.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)      371 2023-05-15 23:27:43.000000 slicpy-0.0.5/slicpy/test.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     1414 2023-05-08 21:07:07.000000 slicpy-0.0.5/slicpy/test_server.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     2984 2023-05-02 16:16:22.000000 slicpy-0.0.5/slicpy/util.py
-drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:22:02.631067 slicpy-0.0.5/slicpy.egg-info/
--rw-r--r--   0 teddyoweh   (501) staff       (20)     6002 2023-05-16 03:22:02.000000 slicpy-0.0.5/slicpy.egg-info/PKG-INFO
--rw-r--r--   0 teddyoweh   (501) staff       (20)      396 2023-05-16 03:22:02.000000 slicpy-0.0.5/slicpy.egg-info/SOURCES.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)        1 2023-05-16 03:22:02.000000 slicpy-0.0.5/slicpy.egg-info/dependency_links.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)       46 2023-05-16 03:22:02.000000 slicpy-0.0.5/slicpy.egg-info/entry_points.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)       29 2023-05-16 03:22:02.000000 slicpy-0.0.5/slicpy.egg-info/requires.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)        7 2023-05-16 03:22:02.000000 slicpy-0.0.5/slicpy.egg-info/top_level.txt
+drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:23:49.553267 slicpy-0.0.6/
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     6004 2023-05-16 03:23:49.553333 slicpy-0.0.6/PKG-INFO
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     5620 2023-05-16 03:22:55.000000 slicpy-0.0.6/README.md
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      107 2023-05-16 03:23:49.553645 slicpy-0.0.6/setup.cfg
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     1002 2023-05-16 03:23:44.000000 slicpy-0.0.6/setup.py
+drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:23:49.552126 slicpy-0.0.6/slicpy/
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     1373 2023-05-02 15:55:53.000000 slicpy-0.0.6/slicpy/Console.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      650 2023-05-15 22:56:23.000000 slicpy-0.0.6/slicpy/HashMap.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     1009 2023-05-15 23:17:16.000000 slicpy-0.0.6/slicpy/NetworkTrafficMap.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      700 2023-05-15 22:55:30.000000 slicpy-0.0.6/slicpy/Rate.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     8357 2023-05-16 03:23:37.000000 slicpy-0.0.6/slicpy/Slic.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      154 2023-05-16 03:21:10.000000 slicpy-0.0.6/slicpy/__init__.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     3015 2023-05-02 11:02:36.000000 slicpy-0.0.6/slicpy/decorators.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      371 2023-05-15 23:27:43.000000 slicpy-0.0.6/slicpy/test.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     1414 2023-05-08 21:07:07.000000 slicpy-0.0.6/slicpy/test_server.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     2984 2023-05-02 16:16:22.000000 slicpy-0.0.6/slicpy/util.py
+drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:23:49.553131 slicpy-0.0.6/slicpy.egg-info/
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     6004 2023-05-16 03:23:49.000000 slicpy-0.0.6/slicpy.egg-info/PKG-INFO
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      396 2023-05-16 03:23:49.000000 slicpy-0.0.6/slicpy.egg-info/SOURCES.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)        1 2023-05-16 03:23:49.000000 slicpy-0.0.6/slicpy.egg-info/dependency_links.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)       46 2023-05-16 03:23:49.000000 slicpy-0.0.6/slicpy.egg-info/entry_points.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)       29 2023-05-16 03:23:49.000000 slicpy-0.0.6/slicpy.egg-info/requires.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)        7 2023-05-16 03:23:49.000000 slicpy-0.0.6/slicpy.egg-info/top_level.txt
```

### Comparing `slicpy-0.0.5/PKG-INFO` & `slicpy-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Swift Low-latency Intercommunication
 Home-page: https://github.com/teddyoweh/SLIC
 Author: Teddy Oweh
 Author-email: teddyoweh@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -27,15 +27,15 @@
 SLIC is designed to simplify client-server communication in Python applications. It enables the creation of resources and handles incoming client requests, allowing for efficient data transfer between the client and server. The library incorporates features such as rate limiting to prevent abuse and network traffic management for tracking and monitoring client connections.
 
 ## Quick Start
 To quickly get started with SLIC, follow these steps:
 
 1. Install SLIC library:
 ```sh
-$ pip install slic
+$ pip install slicpy
 ```
 2. Import the necessary modules and classes:
 ```py
 from slic import Slic, RateLimiter, Rate, NetworkTrafficMap
 ```
 
 3. Create a server instance and define your resources:
```

### Comparing `slicpy-0.0.5/README.md` & `slicpy-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 SLIC is designed to simplify client-server communication in Python applications. It enables the creation of resources and handles incoming client requests, allowing for efficient data transfer between the client and server. The library incorporates features such as rate limiting to prevent abuse and network traffic management for tracking and monitoring client connections.
 
 ## Quick Start
 To quickly get started with SLIC, follow these steps:
 
 1. Install SLIC library:
 ```sh
-$ pip install slic
+$ pip install slicpy
 ```
 2. Import the necessary modules and classes:
 ```py
 from slic import Slic, RateLimiter, Rate, NetworkTrafficMap
 ```
 
 3. Create a server instance and define your resources:
```

### Comparing `slicpy-0.0.5/setup.py` & `slicpy-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 HERE = pathlib.Path(__file__).parent
 
  
 README = (HERE / "README.md").read_text()
  
 setup(
     name="slicpy",
-    version="0.0.5",
+    version="0.0.6",
     description="Swift Low-latency Intercommunication",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/teddyoweh/SLIC",
     author="Teddy Oweh",
     author_email="teddyoweh@gmail.com",
     packages=find_packages(),
```

### Comparing `slicpy-0.0.5/slicpy/Console.py` & `slicpy-0.0.6/slicpy/Console.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.5/slicpy/HashMap.py` & `slicpy-0.0.6/slicpy/HashMap.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.5/slicpy/NetworkTrafficMap.py` & `slicpy-0.0.6/slicpy/NetworkTrafficMap.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.5/slicpy/Rate.py` & `slicpy-0.0.6/slicpy/Rate.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.5/slicpy/Slic.py` & `slicpy-0.0.6/slicpy/Slic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import socket
 import threading
-from decorators import Logger
+from .decorators import Logger
 import ast
-from util import Util
-from HashMap import HashMap
-from NetworkTrafficMap import NetworkTrafficMap
-from Rate import Rate    
+from .util import Util
+from .HashMap import HashMap
+from .NetworkTrafficMap import NetworkTrafficMap
+from .Rate import Rate    
 class RateLimiter(object):
     def __init__(self, Network: NetworkTrafficMap, rate: Rate):
         self.network = Network
         self.rate = rate
 
     def is_allowed(self, addr):
         ip = Util.ipkey(addr)
```

### Comparing `slicpy-0.0.5/slicpy/decorators.py` & `slicpy-0.0.6/slicpy/decorators.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.5/slicpy/test_server.py` & `slicpy-0.0.6/slicpy/test_server.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.5/slicpy/util.py` & `slicpy-0.0.6/slicpy/util.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.5/slicpy.egg-info/PKG-INFO` & `slicpy-0.0.6/slicpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Swift Low-latency Intercommunication
 Home-page: https://github.com/teddyoweh/SLIC
 Author: Teddy Oweh
 Author-email: teddyoweh@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -27,15 +27,15 @@
 SLIC is designed to simplify client-server communication in Python applications. It enables the creation of resources and handles incoming client requests, allowing for efficient data transfer between the client and server. The library incorporates features such as rate limiting to prevent abuse and network traffic management for tracking and monitoring client connections.
 
 ## Quick Start
 To quickly get started with SLIC, follow these steps:
 
 1. Install SLIC library:
 ```sh
-$ pip install slic
+$ pip install slicpy
 ```
 2. Import the necessary modules and classes:
 ```py
 from slic import Slic, RateLimiter, Rate, NetworkTrafficMap
 ```
 
 3. Create a server instance and define your resources:
```

