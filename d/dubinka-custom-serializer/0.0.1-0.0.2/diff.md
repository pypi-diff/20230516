# Comparing `tmp/dubinka-custom-serializer-0.0.1.tar.gz` & `tmp/dubinka-custom-serializer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dubinka-custom-serializer-0.0.1.tar", last modified: Tue May 16 15:12:11 2023, max compression
+gzip compressed data, was "dubinka-custom-serializer-0.0.2.tar", last modified: Tue May 16 15:33:05 2023, max compression
```

## Comparing `dubinka-custom-serializer-0.0.1.tar` & `dubinka-custom-serializer-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:12:11.442694 dubinka-custom-serializer-0.0.1/
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:12:11.442694 dubinka-custom-serializer-0.0.1/PKG-INFO
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:12:11.438694 dubinka-custom-serializer-0.0.1/custom_serializer/
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:12:11.438694 dubinka-custom-serializer-0.0.1/custom_serializer/src/
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 14:58:45.000000 dubinka-custom-serializer-0.0.1/custom_serializer/src/__init__.py
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      406 2023-05-16 13:27:05.000000 dubinka-custom-serializer-0.0.1/custom_serializer/src/serializer_factory.py
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:12:11.438694 dubinka-custom-serializer-0.0.1/dubinka_custom_serializer.egg-info/
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:12:11.000000 dubinka-custom-serializer-0.0.1/dubinka_custom_serializer.egg-info/PKG-INFO
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      334 2023-05-16 15:12:11.000000 dubinka-custom-serializer-0.0.1/dubinka_custom_serializer.egg-info/SOURCES.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)        1 2023-05-16 15:12:11.000000 dubinka-custom-serializer-0.0.1/dubinka_custom_serializer.egg-info/dependency_links.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       83 2023-05-16 15:12:11.000000 dubinka-custom-serializer-0.0.1/dubinka_custom_serializer.egg-info/entry_points.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       18 2023-05-16 15:12:11.000000 dubinka-custom-serializer-0.0.1/dubinka_custom_serializer.egg-info/top_level.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       38 2023-05-16 15:12:11.442694 dubinka-custom-serializer-0.0.1/setup.cfg
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      379 2023-05-16 15:02:35.000000 dubinka-custom-serializer-0.0.1/setup.py
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:33:05.098127 dubinka-custom-serializer-0.0.2/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:33:05.098127 dubinka-custom-serializer-0.0.2/PKG-INFO
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:33:05.098127 dubinka-custom-serializer-0.0.2/custom_serializer/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:00:18.000000 dubinka-custom-serializer-0.0.2/custom_serializer/__init__.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      732 2023-05-16 15:08:50.000000 dubinka-custom-serializer-0.0.2/custom_serializer/custom_serializer.py
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:33:05.098127 dubinka-custom-serializer-0.0.2/custom_serializer/src/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 14:58:45.000000 dubinka-custom-serializer-0.0.2/custom_serializer/src/__init__.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      406 2023-05-16 13:27:05.000000 dubinka-custom-serializer-0.0.2/custom_serializer/src/serializer_factory.py
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:33:05.098127 dubinka-custom-serializer-0.0.2/dubinka_custom_serializer.egg-info/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:33:05.000000 dubinka-custom-serializer-0.0.2/dubinka_custom_serializer.egg-info/PKG-INFO
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      403 2023-05-16 15:33:05.000000 dubinka-custom-serializer-0.0.2/dubinka_custom_serializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)        1 2023-05-16 15:33:05.000000 dubinka-custom-serializer-0.0.2/dubinka_custom_serializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       79 2023-05-16 15:33:05.000000 dubinka-custom-serializer-0.0.2/dubinka_custom_serializer.egg-info/entry_points.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       18 2023-05-16 15:33:05.000000 dubinka-custom-serializer-0.0.2/dubinka_custom_serializer.egg-info/top_level.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       38 2023-05-16 15:33:05.098127 dubinka-custom-serializer-0.0.2/setup.cfg
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      371 2023-05-16 15:27:40.000000 dubinka-custom-serializer-0.0.2/setup.py
```

