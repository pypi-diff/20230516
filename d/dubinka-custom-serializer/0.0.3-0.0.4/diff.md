# Comparing `tmp/dubinka-custom-serializer-0.0.3.tar.gz` & `tmp/dubinka-custom-serializer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dubinka-custom-serializer-0.0.3.tar", last modified: Tue May 16 15:41:48 2023, max compression
+gzip compressed data, was "dubinka-custom-serializer-0.0.4.tar", last modified: Tue May 16 15:45:01 2023, max compression
```

## Comparing `dubinka-custom-serializer-0.0.3.tar` & `dubinka-custom-serializer-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:41:48.360170 dubinka-custom-serializer-0.0.3/
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:41:48.360170 dubinka-custom-serializer-0.0.3/PKG-INFO
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:41:48.360170 dubinka-custom-serializer-0.0.3/custom_serializer/
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       83 2023-05-16 15:40:24.000000 dubinka-custom-serializer-0.0.3/custom_serializer/__init__.py
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      728 2023-05-16 15:39:00.000000 dubinka-custom-serializer-0.0.3/custom_serializer/custom_serializer.py
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      406 2023-05-16 13:27:05.000000 dubinka-custom-serializer-0.0.3/custom_serializer/serializer_factory.py
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:41:48.360170 dubinka-custom-serializer-0.0.3/dubinka_custom_serializer.egg-info/
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:41:48.000000 dubinka-custom-serializer-0.0.3/dubinka_custom_serializer.egg-info/PKG-INFO
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      365 2023-05-16 15:41:48.000000 dubinka-custom-serializer-0.0.3/dubinka_custom_serializer.egg-info/SOURCES.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)        1 2023-05-16 15:41:48.000000 dubinka-custom-serializer-0.0.3/dubinka_custom_serializer.egg-info/dependency_links.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       79 2023-05-16 15:41:48.000000 dubinka-custom-serializer-0.0.3/dubinka_custom_serializer.egg-info/entry_points.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       18 2023-05-16 15:41:48.000000 dubinka-custom-serializer-0.0.3/dubinka_custom_serializer.egg-info/top_level.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       38 2023-05-16 15:41:48.360170 dubinka-custom-serializer-0.0.3/setup.cfg
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      371 2023-05-16 15:41:32.000000 dubinka-custom-serializer-0.0.3/setup.py
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:45:01.748151 dubinka-custom-serializer-0.0.4/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:45:01.748151 dubinka-custom-serializer-0.0.4/PKG-INFO
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:45:01.744151 dubinka-custom-serializer-0.0.4/custom_serializer/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       83 2023-05-16 15:40:24.000000 dubinka-custom-serializer-0.0.4/custom_serializer/__init__.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      706 2023-05-16 15:44:59.000000 dubinka-custom-serializer-0.0.4/custom_serializer/custom_serializer.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      406 2023-05-16 13:27:05.000000 dubinka-custom-serializer-0.0.4/custom_serializer/serializer_factory.py
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:45:01.748151 dubinka-custom-serializer-0.0.4/dubinka_custom_serializer.egg-info/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:45:01.000000 dubinka-custom-serializer-0.0.4/dubinka_custom_serializer.egg-info/PKG-INFO
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      365 2023-05-16 15:45:01.000000 dubinka-custom-serializer-0.0.4/dubinka_custom_serializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)        1 2023-05-16 15:45:01.000000 dubinka-custom-serializer-0.0.4/dubinka_custom_serializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       79 2023-05-16 15:45:01.000000 dubinka-custom-serializer-0.0.4/dubinka_custom_serializer.egg-info/entry_points.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       18 2023-05-16 15:45:01.000000 dubinka-custom-serializer-0.0.4/dubinka_custom_serializer.egg-info/top_level.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       38 2023-05-16 15:45:01.748151 dubinka-custom-serializer-0.0.4/setup.cfg
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      371 2023-05-16 15:44:59.000000 dubinka-custom-serializer-0.0.4/setup.py
```

### Comparing `dubinka-custom-serializer-0.0.3/custom_serializer/custom_serializer.py` & `dubinka-custom-serializer-0.0.4/custom_serializer/custom_serializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from lab3.custom_serializer.serializer_factory import SerializerFactory
+from .serializer_factory import SerializerFactory
 
 
 def main():
     args = sys.argv
 
     if len(args) != 5:
         print("Invalid amount of arguments")
```

