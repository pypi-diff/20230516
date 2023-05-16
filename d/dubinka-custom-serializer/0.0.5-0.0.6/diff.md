# Comparing `tmp/dubinka-custom-serializer-0.0.5.tar.gz` & `tmp/dubinka-custom-serializer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dubinka-custom-serializer-0.0.5.tar", last modified: Tue May 16 15:48:31 2023, max compression
+gzip compressed data, was "dubinka-custom-serializer-0.0.6.tar", last modified: Tue May 16 15:50:51 2023, max compression
```

## Comparing `dubinka-custom-serializer-0.0.5.tar` & `dubinka-custom-serializer-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:48:31.847545 dubinka-custom-serializer-0.0.5/
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:48:31.843545 dubinka-custom-serializer-0.0.5/PKG-INFO
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:48:31.843545 dubinka-custom-serializer-0.0.5/custom_serializer/
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       50 2023-05-16 15:47:40.000000 dubinka-custom-serializer-0.0.5/custom_serializer/__init__.py
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      706 2023-05-16 15:44:59.000000 dubinka-custom-serializer-0.0.5/custom_serializer/custom_serializer.py
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      406 2023-05-16 13:27:05.000000 dubinka-custom-serializer-0.0.5/custom_serializer/serializer_factory.py
-drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:48:31.843545 dubinka-custom-serializer-0.0.5/dubinka_custom_serializer.egg-info/
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:48:31.000000 dubinka-custom-serializer-0.0.5/dubinka_custom_serializer.egg-info/PKG-INFO
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      365 2023-05-16 15:48:31.000000 dubinka-custom-serializer-0.0.5/dubinka_custom_serializer.egg-info/SOURCES.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)        1 2023-05-16 15:48:31.000000 dubinka-custom-serializer-0.0.5/dubinka_custom_serializer.egg-info/dependency_links.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       79 2023-05-16 15:48:31.000000 dubinka-custom-serializer-0.0.5/dubinka_custom_serializer.egg-info/entry_points.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       18 2023-05-16 15:48:31.000000 dubinka-custom-serializer-0.0.5/dubinka_custom_serializer.egg-info/top_level.txt
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       38 2023-05-16 15:48:31.847545 dubinka-custom-serializer-0.0.5/setup.cfg
--rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      371 2023-05-16 15:48:28.000000 dubinka-custom-serializer-0.0.5/setup.py
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:50:51.281383 dubinka-custom-serializer-0.0.6/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:50:51.281383 dubinka-custom-serializer-0.0.6/PKG-INFO
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:50:51.281383 dubinka-custom-serializer-0.0.6/custom_serializer/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       50 2023-05-16 15:47:40.000000 dubinka-custom-serializer-0.0.6/custom_serializer/__init__.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      706 2023-05-16 15:44:59.000000 dubinka-custom-serializer-0.0.6/custom_serializer/custom_serializer.py
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:50:51.281383 dubinka-custom-serializer-0.0.6/custom_serializer/encoder/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       63 2023-05-16 13:34:05.000000 dubinka-custom-serializer-0.0.6/custom_serializer/encoder/__init__.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      505 2023-05-15 19:41:03.000000 dubinka-custom-serializer-0.0.6/custom_serializer/encoder/constants.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)     8394 2023-05-16 13:32:46.000000 dubinka-custom-serializer-0.0.6/custom_serializer/encoder/encoder.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      406 2023-05-16 13:27:05.000000 dubinka-custom-serializer-0.0.6/custom_serializer/serializer_factory.py
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:50:51.281383 dubinka-custom-serializer-0.0.6/custom_serializer/serializers/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       61 2023-05-16 13:29:26.000000 dubinka-custom-serializer-0.0.6/custom_serializer/serializers/__init__.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)     3100 2023-05-16 14:16:02.000000 dubinka-custom-serializer-0.0.6/custom_serializer/serializers/json_serializer.py
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)     3099 2023-05-16 14:19:33.000000 dubinka-custom-serializer-0.0.6/custom_serializer/serializers/xml_serializer.py
+drwxrwxr-x   0 mikhail   (1000) mikhail   (1000)        0 2023-05-16 15:50:51.281383 dubinka-custom-serializer-0.0.6/dubinka_custom_serializer.egg-info/
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      189 2023-05-16 15:50:51.000000 dubinka-custom-serializer-0.0.6/dubinka_custom_serializer.egg-info/PKG-INFO
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      618 2023-05-16 15:50:51.000000 dubinka-custom-serializer-0.0.6/dubinka_custom_serializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)        1 2023-05-16 15:50:51.000000 dubinka-custom-serializer-0.0.6/dubinka_custom_serializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       79 2023-05-16 15:50:51.000000 dubinka-custom-serializer-0.0.6/dubinka_custom_serializer.egg-info/entry_points.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       18 2023-05-16 15:50:51.000000 dubinka-custom-serializer-0.0.6/dubinka_custom_serializer.egg-info/top_level.txt
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)       38 2023-05-16 15:50:51.281383 dubinka-custom-serializer-0.0.6/setup.cfg
+-rw-rw-r--   0 mikhail   (1000) mikhail   (1000)      461 2023-05-16 15:50:49.000000 dubinka-custom-serializer-0.0.6/setup.py
```

### Comparing `dubinka-custom-serializer-0.0.5/custom_serializer/custom_serializer.py` & `dubinka-custom-serializer-0.0.6/custom_serializer/custom_serializer.py`

 * *Files identical despite different names*

