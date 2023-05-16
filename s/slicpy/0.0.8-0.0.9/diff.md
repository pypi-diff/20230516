# Comparing `tmp/slicpy-0.0.8.tar.gz` & `tmp/slicpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicpy-0.0.8.tar", last modified: Tue May 16 03:29:16 2023, max compression
+gzip compressed data, was "slicpy-0.0.9.tar", last modified: Tue May 16 03:42:09 2023, max compression
```

## Comparing `slicpy-0.0.8.tar` & `slicpy-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:29:16.830519 slicpy-0.0.8/
--rw-r--r--   0 teddyoweh   (501) staff       (20)     6004 2023-05-16 03:29:16.830584 slicpy-0.0.8/PKG-INFO
--rw-r--r--   0 teddyoweh   (501) staff       (20)     5620 2023-05-16 03:22:55.000000 slicpy-0.0.8/README.md
--rw-r--r--   0 teddyoweh   (501) staff       (20)      107 2023-05-16 03:29:16.830902 slicpy-0.0.8/setup.cfg
--rw-r--r--   0 teddyoweh   (501) staff       (20)     1002 2023-05-16 03:29:09.000000 slicpy-0.0.8/setup.py
-drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:29:16.829292 slicpy-0.0.8/slicpy/
--rw-r--r--   0 teddyoweh   (501) staff       (20)     1373 2023-05-02 15:55:53.000000 slicpy-0.0.8/slicpy/Console.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)      650 2023-05-15 22:56:23.000000 slicpy-0.0.8/slicpy/HashMap.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     1011 2023-05-16 03:25:35.000000 slicpy-0.0.8/slicpy/NetworkTrafficMap.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)      700 2023-05-15 22:55:30.000000 slicpy-0.0.8/slicpy/Rate.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     8357 2023-05-16 03:23:37.000000 slicpy-0.0.8/slicpy/Slic.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)      154 2023-05-16 03:21:10.000000 slicpy-0.0.8/slicpy/__init__.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     2995 2023-05-16 03:29:06.000000 slicpy-0.0.8/slicpy/decorators.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)      371 2023-05-15 23:27:43.000000 slicpy-0.0.8/slicpy/test.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     1414 2023-05-08 21:07:07.000000 slicpy-0.0.8/slicpy/test_server.py
--rw-r--r--   0 teddyoweh   (501) staff       (20)     2984 2023-05-02 16:16:22.000000 slicpy-0.0.8/slicpy/util.py
-drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:29:16.830374 slicpy-0.0.8/slicpy.egg-info/
--rw-r--r--   0 teddyoweh   (501) staff       (20)     6004 2023-05-16 03:29:16.000000 slicpy-0.0.8/slicpy.egg-info/PKG-INFO
--rw-r--r--   0 teddyoweh   (501) staff       (20)      396 2023-05-16 03:29:16.000000 slicpy-0.0.8/slicpy.egg-info/SOURCES.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)        1 2023-05-16 03:29:16.000000 slicpy-0.0.8/slicpy.egg-info/dependency_links.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)       46 2023-05-16 03:29:16.000000 slicpy-0.0.8/slicpy.egg-info/entry_points.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)       29 2023-05-16 03:29:16.000000 slicpy-0.0.8/slicpy.egg-info/requires.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)        7 2023-05-16 03:29:16.000000 slicpy-0.0.8/slicpy.egg-info/top_level.txt
+drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:42:09.816654 slicpy-0.0.9/
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     6004 2023-05-16 03:42:09.816735 slicpy-0.0.9/PKG-INFO
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     5620 2023-05-16 03:22:55.000000 slicpy-0.0.9/README.md
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      107 2023-05-16 03:42:09.817089 slicpy-0.0.9/setup.cfg
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     1002 2023-05-16 03:41:46.000000 slicpy-0.0.9/setup.py
+drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:42:09.815317 slicpy-0.0.9/slicpy/
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     1373 2023-05-02 15:55:53.000000 slicpy-0.0.9/slicpy/Console.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      650 2023-05-15 22:56:23.000000 slicpy-0.0.9/slicpy/HashMap.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     1011 2023-05-16 03:25:35.000000 slicpy-0.0.9/slicpy/NetworkTrafficMap.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      700 2023-05-15 22:55:30.000000 slicpy-0.0.9/slicpy/Rate.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     8358 2023-05-16 03:40:09.000000 slicpy-0.0.9/slicpy/Slic.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      154 2023-05-16 03:21:10.000000 slicpy-0.0.9/slicpy/__init__.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     3004 2023-05-16 03:41:41.000000 slicpy-0.0.9/slicpy/decorators.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      371 2023-05-15 23:27:43.000000 slicpy-0.0.9/slicpy/test.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     1414 2023-05-08 21:07:07.000000 slicpy-0.0.9/slicpy/test_server.py
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     2984 2023-05-02 16:16:22.000000 slicpy-0.0.9/slicpy/util.py
+drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 03:42:09.816533 slicpy-0.0.9/slicpy.egg-info/
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     6004 2023-05-16 03:42:09.000000 slicpy-0.0.9/slicpy.egg-info/PKG-INFO
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      396 2023-05-16 03:42:09.000000 slicpy-0.0.9/slicpy.egg-info/SOURCES.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)        1 2023-05-16 03:42:09.000000 slicpy-0.0.9/slicpy.egg-info/dependency_links.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)       46 2023-05-16 03:42:09.000000 slicpy-0.0.9/slicpy.egg-info/entry_points.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)       29 2023-05-16 03:42:09.000000 slicpy-0.0.9/slicpy.egg-info/requires.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)        7 2023-05-16 03:42:09.000000 slicpy-0.0.9/slicpy.egg-info/top_level.txt
```

### Comparing `slicpy-0.0.8/PKG-INFO` & `slicpy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Swift Low-latency Intercommunication
 Home-page: https://github.com/teddyoweh/SLIC
 Author: Teddy Oweh
 Author-email: teddyoweh@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `slicpy-0.0.8/README.md` & `slicpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.8/setup.py` & `slicpy-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 HERE = pathlib.Path(__file__).parent
 
  
 README = (HERE / "README.md").read_text()
  
 setup(
     name="slicpy",
-    version="0.0.8",
+    version="0.0.9",
     description="Swift Low-latency Intercommunication",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/teddyoweh/SLIC",
     author="Teddy Oweh",
     author_email="teddyoweh@gmail.com",
     packages=find_packages(),
```

### Comparing `slicpy-0.0.8/slicpy/Console.py` & `slicpy-0.0.9/slicpy/Console.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.8/slicpy/HashMap.py` & `slicpy-0.0.9/slicpy/HashMap.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.8/slicpy/NetworkTrafficMap.py` & `slicpy-0.0.9/slicpy/NetworkTrafficMap.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.8/slicpy/Rate.py` & `slicpy-0.0.9/slicpy/Rate.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.8/slicpy/Slic.py` & `slicpy-0.0.9/slicpy/Slic.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     logger = Logger("server_logs.log")
     def __init__(self):
 
         super().__init__(socket.AF_INET, socket.SOCK_STREAM)
         #self.logger = Logger("logs/server_logs.log")
         self.resources = HashMap()
         self.network_traffic  = NetworkTrafficMap()
-        self.rate_limiter = RateLimiter(self.network_traffic)
+        #self.rate_limiter = RateLimiter(self.network_traffic)
         
     @logger.decorator   
     def start(self,host:str,port:int):
         self.bind((host,port))
         self.listen(5)
         while True:
             conn, addr = self.accept()
```

### Comparing `slicpy-0.0.8/slicpy/decorators.py` & `slicpy-0.0.9/slicpy/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import functools
 from datetime import datetime
 import inspect
 class Logger:
     def __init__(self, log_path):
         self.log_path = '@logs/'+ log_path
-        self.create_log_file()
+        
         try:
             os.mkdir('@logs')
         except:
             pass
+        self.create_log_file()
 
     def create_log_file(self):
         if not os.path.exists(self.log_path):
 
             open(self.log_path, 'w').write("")
```

### Comparing `slicpy-0.0.8/slicpy/test_server.py` & `slicpy-0.0.9/slicpy/test_server.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.8/slicpy/util.py` & `slicpy-0.0.9/slicpy/util.py`

 * *Files identical despite different names*

### Comparing `slicpy-0.0.8/slicpy.egg-info/PKG-INFO` & `slicpy-0.0.9/slicpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Swift Low-latency Intercommunication
 Home-page: https://github.com/teddyoweh/SLIC
 Author: Teddy Oweh
 Author-email: teddyoweh@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

