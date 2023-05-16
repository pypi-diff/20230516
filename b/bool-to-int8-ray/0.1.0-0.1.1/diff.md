# Comparing `tmp/bool-to-int8-ray-0.1.0.tar.gz` & `tmp/bool-to-int8-ray-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bool-to-int8-ray-0.1.0.tar", last modified: Fri May 12 06:16:45 2023, max compression
+gzip compressed data, was "bool-to-int8-ray-0.1.1.tar", last modified: Tue May 16 13:13:11 2023, max compression
```

## Comparing `bool-to-int8-ray-0.1.0.tar` & `bool-to-int8-ray-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-12 06:16:45.227985 bool-to-int8-ray-0.1.0/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.1.0/LICENSE
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.1.0/MANIFEST.in
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     2879 2023-05-12 06:16:45.227985 bool-to-int8-ray-0.1.0/PKG-INFO
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     2530 2023-05-09 16:05:24.000000 bool-to-int8-ray-0.1.0/README.md
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-12 06:16:45.223986 bool-to-int8-ray-0.1.0/bool_to_int8_ray/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      116 2023-05-09 15:03:39.000000 bool-to-int8-ray-0.1.0/bool_to_int8_ray/__init__.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     2032 2023-05-09 16:03:37.000000 bool-to-int8-ray-0.1.0/bool_to_int8_ray/serialize.py
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-12 06:16:45.223986 bool-to-int8-ray-0.1.0/bool_to_int8_ray.egg-info/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     2879 2023-05-12 06:16:45.000000 bool-to-int8-ray-0.1.0/bool_to_int8_ray.egg-info/PKG-INFO
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      389 2023-05-12 06:16:45.000000 bool-to-int8-ray-0.1.0/bool_to_int8_ray.egg-info/SOURCES.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-05-12 06:16:45.000000 bool-to-int8-ray-0.1.0/bool_to_int8_ray.egg-info/dependency_links.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       37 2023-05-12 06:16:45.000000 bool-to-int8-ray-0.1.0/bool_to_int8_ray.egg-info/requires.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       17 2023-05-12 06:16:45.000000 bool-to-int8-ray-0.1.0/bool_to_int8_ray.egg-info/top_level.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-05-09 16:04:11.000000 bool-to-int8-ray-0.1.0/bool_to_int8_ray.egg-info/zip-safe
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-05-12 06:16:45.227985 bool-to-int8-ray-0.1.0/setup.cfg
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     1048 2023-05-09 14:24:59.000000 bool-to-int8-ray-0.1.0/setup.py
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-12 06:16:45.227985 bool-to-int8-ray-0.1.0/test/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.1.0/test/__init__.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     1544 2023-05-09 15:52:41.000000 bool-to-int8-ray-0.1.0/test/speedtest.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      657 2023-05-09 15:45:00.000000 bool-to-int8-ray-0.1.0/test/test_serialize.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.1.1/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.1.1/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2879 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2530 2023-05-16 13:12:58.000000 bool-to-int8-ray-0.1.1/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/bool_to_int8_ray/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      116 2023-05-16 13:12:58.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2178 2023-05-16 13:12:58.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray/serialize.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2879 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      389 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       37 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       17 2023-05-16 13:13:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-05-09 16:04:11.000000 bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1048 2023-05-09 14:24:59.000000 bool-to-int8-ray-0.1.1/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-16 13:13:11.993179 bool-to-int8-ray-0.1.1/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-05-09 13:33:12.000000 bool-to-int8-ray-0.1.1/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1544 2023-05-09 15:52:41.000000 bool-to-int8-ray-0.1.1/test/speedtest.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      657 2023-05-09 15:45:00.000000 bool-to-int8-ray-0.1.1/test/test_serialize.py
```

### Comparing `bool-to-int8-ray-0.1.0/LICENSE` & `bool-to-int8-ray-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bool-to-int8-ray-0.1.0/PKG-INFO` & `bool-to-int8-ray-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bool-to-int8-ray
-Version: 0.1.0
+Version: 0.1.1
 Summary: bool to int8 serialization with ray.io
 Home-page: http://github.com/satzbeleg/bool-to-int8-ray
 Author: Ulf Hamster
 Author-email: 554c46@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `bool-to-int8-ray-0.1.0/README.md` & `bool-to-int8-ray-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bool-to-int8-ray-0.1.0/bool_to_int8_ray/serialize.py` & `bool-to-int8-ray-0.1.1/bool_to_int8_ray/serialize.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 import ray
 import os
 import psutil
 import gc
 
 
 logger = logging.getLogger(__name__)
+logging.basicConfig(
+    level=logging.DEBUG,
+    format="%(asctime)s - %(levelname)s - %(name)s: %(message)s",
+    datefmt="%y-%m-%d %H:%M:%S"
+)
 
 PCT_CPU = float(os.environ.get("B2I8_PCT_CPU", "0.9"))
 NUM_CPU = os.environ.get("B2I8_NUM_CPU")
 if NUM_CPU is None:
     NUM_CPU = max(1, int(psutil.cpu_count(logical=False) * PCT_CPU))
 ray.init(num_cpus=NUM_CPU)
```

### Comparing `bool-to-int8-ray-0.1.0/bool_to_int8_ray.egg-info/PKG-INFO` & `bool-to-int8-ray-0.1.1/bool_to_int8_ray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bool-to-int8-ray
-Version: 0.1.0
+Version: 0.1.1
 Summary: bool to int8 serialization with ray.io
 Home-page: http://github.com/satzbeleg/bool-to-int8-ray
 Author: Ulf Hamster
 Author-email: 554c46@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `bool-to-int8-ray-0.1.0/setup.py` & `bool-to-int8-ray-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `bool-to-int8-ray-0.1.0/test/speedtest.py` & `bool-to-int8-ray-0.1.1/test/speedtest.py`

 * *Files identical despite different names*

### Comparing `bool-to-int8-ray-0.1.0/test/test_serialize.py` & `bool-to-int8-ray-0.1.1/test/test_serialize.py`

 * *Files identical despite different names*

