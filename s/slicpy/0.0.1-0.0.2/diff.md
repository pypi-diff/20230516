# Comparing `tmp/slicpy-0.0.1.tar.gz` & `tmp/slicpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicpy-0.0.1.tar", last modified: Mon May 15 23:49:27 2023, max compression
+gzip compressed data, was "slicpy-0.0.2.tar", last modified: Tue May 16 02:56:59 2023, max compression
```

## Comparing `slicpy-0.0.1.tar` & `slicpy-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-15 23:49:27.485579 slicpy-0.0.1/
--rw-r--r--   0 teddyoweh   (501) staff       (20)     6058 2023-05-15 23:49:27.485644 slicpy-0.0.1/PKG-INFO
--rw-r--r--   0 teddyoweh   (501) staff       (20)     5673 2023-05-15 23:34:18.000000 slicpy-0.0.1/README.md
--rw-r--r--   0 teddyoweh   (501) staff       (20)       38 2023-05-15 23:49:27.485846 slicpy-0.0.1/setup.cfg
--rw-r--r--   0 teddyoweh   (501) staff       (20)     1003 2023-05-15 23:49:11.000000 slicpy-0.0.1/setup.py
-drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-15 23:49:27.485424 slicpy-0.0.1/slicpy.egg-info/
--rw-r--r--   0 teddyoweh   (501) staff       (20)     6058 2023-05-15 23:49:27.000000 slicpy-0.0.1/slicpy.egg-info/PKG-INFO
--rw-r--r--   0 teddyoweh   (501) staff       (20)      210 2023-05-15 23:49:27.000000 slicpy-0.0.1/slicpy.egg-info/SOURCES.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)        1 2023-05-15 23:49:27.000000 slicpy-0.0.1/slicpy.egg-info/dependency_links.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)       46 2023-05-15 23:49:27.000000 slicpy-0.0.1/slicpy.egg-info/entry_points.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)       29 2023-05-15 23:49:27.000000 slicpy-0.0.1/slicpy.egg-info/requires.txt
--rw-r--r--   0 teddyoweh   (501) staff       (20)        1 2023-05-15 23:49:27.000000 slicpy-0.0.1/slicpy.egg-info/top_level.txt
+drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 02:56:59.652580 slicpy-0.0.2/
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     6601 2023-05-16 02:56:59.652635 slicpy-0.0.2/PKG-INFO
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     6216 2023-05-16 02:56:44.000000 slicpy-0.0.2/README.md
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      107 2023-05-16 02:56:59.652870 slicpy-0.0.2/setup.cfg
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     1003 2023-05-16 02:54:35.000000 slicpy-0.0.2/setup.py
+drwxr-xr-x   0 teddyoweh   (501) staff       (20)        0 2023-05-16 02:56:59.652476 slicpy-0.0.2/slicpy.egg-info/
+-rw-r--r--   0 teddyoweh   (501) staff       (20)     6601 2023-05-16 02:56:59.000000 slicpy-0.0.2/slicpy.egg-info/PKG-INFO
+-rw-r--r--   0 teddyoweh   (501) staff       (20)      210 2023-05-16 02:56:59.000000 slicpy-0.0.2/slicpy.egg-info/SOURCES.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)        1 2023-05-16 02:56:59.000000 slicpy-0.0.2/slicpy.egg-info/dependency_links.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)       46 2023-05-16 02:56:59.000000 slicpy-0.0.2/slicpy.egg-info/entry_points.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)       29 2023-05-16 02:56:59.000000 slicpy-0.0.2/slicpy.egg-info/requires.txt
+-rw-r--r--   0 teddyoweh   (501) staff       (20)        1 2023-05-16 02:56:59.000000 slicpy-0.0.2/slicpy.egg-info/top_level.txt
```

### Comparing `slicpy-0.0.1/PKG-INFO` & `slicpy-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-Metadata-Version: 2.1
-Name: slicpy
-Version: 0.0.1
-Summary: Swift Low-latency Intercommunication)
-Home-page: https://github.com/teddyoweh/SLIC
-Author: Teddy Oweh
-Author-email: teddyoweh@gmail.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-
 # SLIC - (Swift Low-latency Intercommunication)
+
 SLIC (Swift Low-latency Intercommunication) simplifies client-server communication using tcp / p2p protocols while focusing on latency reduction through low-latency intercommunication techniques. By optimizing network protocols, minimizing data processing overhead, and utilizing efficient data transmission strategies, SLIC ensures faster response times, reduced communication delays, and enhanced overall performance in latency-sensitive applications. 
--
+
+
+
+
+SLIC (Swift Low-latency Intercommunication) simplifies client-server communication using tcp / p2p protocols while focusing on latency reduction through low-latency intercommunication techniques. By optimizing network protocols, minimizing data processing overhead, and utilizing efficient data transmission strategies, SLIC ensures faster response times, reduced communication delays, and enhanced overall performance in latency-sensitive applications.
+
 Additionally, SLIC streamlines Python applications' client-server communication with optimized algorithms for data serialization and deserialization, reducing processing overhead and improving efficiency, while offering built-in capabilities like rate limiting and network traffic management for enhanced network efficiency and seamless data exchange.
 
 ## Table of Contents
-- Introduction
-- Quick Start
-- Features
-- Usage
-- Contributing
-- License
+- [Introduction](./#Introduction)
+- [Quick Start](./#quick-start)
+- [Features](./#Features)
+- [Usage](./#Usage)
+- [Contributing](./#Contributing)
+- [License](./#License)
 
 
 ## Introduction
 SLIC is designed to simplify client-server communication in Python applications. It enables the creation of resources and handles incoming client requests, allowing for efficient data transfer between the client and server. The library incorporates features such as rate limiting to prevent abuse and network traffic management for tracking and monitoring client connections.
 
 ## Quick Start
 To quickly get started with SLIC, follow these steps:
@@ -176,18 +170,18 @@
 # Start the server on a specific host and port
 server.start('localhost', 9999)
 ```
 
 ### Example Client
 To make requests to the SLIC server, you can use the SLIC client:
 ```py
-from slic import SlicClient
+from slic import Slic
 
 # Create a SLIC client instance
-client = SlicClient()
+client = Slic()
 
 # Connect to the SLIC server
 client.connect('localhost', 9999)
 
 # Send a request to the server
 response = client.get_resource(':add', {'a': 10})
 print(response)  # {'answer': 11}
```

### Comparing `slicpy-0.0.1/setup.py` & `slicpy-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 HERE = pathlib.Path(__file__).parent
 
  
 README = (HERE / "README.md").read_text()
  
 setup(
     name="slicpy",
-    version="0.0.1",
+    version="0.0.2",
     description="Swift Low-latency Intercommunication)",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/teddyoweh/SLIC",
     author="Teddy Oweh",
     author_email="teddyoweh@gmail.com",
     packages=find_packages(),
```

### Comparing `slicpy-0.0.1/slicpy.egg-info/PKG-INFO` & `slicpy-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: slicpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Swift Low-latency Intercommunication)
 Home-page: https://github.com/teddyoweh/SLIC
 Author: Teddy Oweh
 Author-email: teddyoweh@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
 # SLIC - (Swift Low-latency Intercommunication)
+
 SLIC (Swift Low-latency Intercommunication) simplifies client-server communication using tcp / p2p protocols while focusing on latency reduction through low-latency intercommunication techniques. By optimizing network protocols, minimizing data processing overhead, and utilizing efficient data transmission strategies, SLIC ensures faster response times, reduced communication delays, and enhanced overall performance in latency-sensitive applications. 
--
+
+
+
+
+SLIC (Swift Low-latency Intercommunication) simplifies client-server communication using tcp / p2p protocols while focusing on latency reduction through low-latency intercommunication techniques. By optimizing network protocols, minimizing data processing overhead, and utilizing efficient data transmission strategies, SLIC ensures faster response times, reduced communication delays, and enhanced overall performance in latency-sensitive applications.
+
 Additionally, SLIC streamlines Python applications' client-server communication with optimized algorithms for data serialization and deserialization, reducing processing overhead and improving efficiency, while offering built-in capabilities like rate limiting and network traffic management for enhanced network efficiency and seamless data exchange.
 
 ## Table of Contents
-- Introduction
-- Quick Start
-- Features
-- Usage
-- Contributing
-- License
+- [Introduction](./#Introduction)
+- [Quick Start](./#quick-start)
+- [Features](./#Features)
+- [Usage](./#Usage)
+- [Contributing](./#Contributing)
+- [License](./#License)
 
 
 ## Introduction
 SLIC is designed to simplify client-server communication in Python applications. It enables the creation of resources and handles incoming client requests, allowing for efficient data transfer between the client and server. The library incorporates features such as rate limiting to prevent abuse and network traffic management for tracking and monitoring client connections.
 
 ## Quick Start
 To quickly get started with SLIC, follow these steps:
@@ -176,18 +182,18 @@
 # Start the server on a specific host and port
 server.start('localhost', 9999)
 ```
 
 ### Example Client
 To make requests to the SLIC server, you can use the SLIC client:
 ```py
-from slic import SlicClient
+from slic import Slic
 
 # Create a SLIC client instance
-client = SlicClient()
+client = Slic()
 
 # Connect to the SLIC server
 client.connect('localhost', 9999)
 
 # Send a request to the server
 response = client.get_resource(':add', {'a': 10})
 print(response)  # {'answer': 11}
```

