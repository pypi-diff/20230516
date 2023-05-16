# Comparing `tmp/kolyaklimkLab3-3.0.0.tar.gz` & `tmp/kolyaklimkLab3-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolyaklimkLab3-3.0.0.tar", last modified: Tue May 16 08:23:12 2023, max compression
+gzip compressed data, was "kolyaklimkLab3-4.0.0.tar", last modified: Tue May 16 08:24:43 2023, max compression
```

## Comparing `kolyaklimkLab3-3.0.0.tar` & `kolyaklimkLab3-4.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:23:12.236993 kolyaklimkLab3-3.0.0/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      117 2023-05-16 08:23:12.236993 kolyaklimkLab3-3.0.0/PKG-INFO
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:23:12.236993 kolyaklimkLab3-3.0.0/kolyaklimkLab3/
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:23:12.236993 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     1510 2023-05-15 22:04:44.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/Constants.py
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:23:12.236993 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/JsonParser/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      682 2023-05-15 21:19:59.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/JsonParser/Constants.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     2802 2023-05-16 07:57:06.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/JsonParser/Json.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      192 2023-05-16 07:57:06.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/JsonParser/__init__.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     7369 2023-05-16 07:57:06.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/Parser.py
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:23:12.236993 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/XmlParser/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      857 2023-05-15 21:40:36.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/XmlParser/Constants.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     3074 2023-05-16 07:57:06.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/XmlParser/Xml.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      162 2023-05-16 08:02:55.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/XmlParser/__init__.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      405 2023-05-16 08:04:59.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/__init__.py
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:23:12.236993 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MySerializer/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      466 2023-05-16 07:57:06.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MySerializer/Factory.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      418 2023-05-15 21:35:45.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MySerializer/Serializer.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      134 2023-05-16 07:57:06.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/MySerializer/__init__.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:21:31.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3/__init__.py
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:23:12.236993 kolyaklimkLab3-3.0.0/kolyaklimkLab3.egg-info/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      117 2023-05-16 08:23:12.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3.egg-info/PKG-INFO
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      734 2023-05-16 08:23:12.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3.egg-info/SOURCES.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 08:23:12.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3.egg-info/dependency_links.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 08:23:12.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3.egg-info/not-zip-safe
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       15 2023-05-16 08:23:12.000000 kolyaklimkLab3-3.0.0/kolyaklimkLab3.egg-info/top_level.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       38 2023-05-16 08:23:12.236993 kolyaklimkLab3-3.0.0/setup.cfg
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      421 2023-05-16 08:23:10.000000 kolyaklimkLab3-3.0.0/setup.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:24:43.138650 kolyaklimkLab3-4.0.0/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       93 2023-05-16 08:24:43.138650 kolyaklimkLab3-4.0.0/PKG-INFO
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:24:43.134650 kolyaklimkLab3-4.0.0/kolyaklimkLab3/
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:24:43.138650 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     1510 2023-05-15 22:04:44.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/Constants.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:24:43.138650 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/JsonParser/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      682 2023-05-15 21:19:59.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/JsonParser/Constants.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     2802 2023-05-16 07:57:06.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/JsonParser/Json.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      192 2023-05-16 07:57:06.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/JsonParser/__init__.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     7369 2023-05-16 07:57:06.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/Parser.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:24:43.138650 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/XmlParser/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      857 2023-05-15 21:40:36.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/XmlParser/Constants.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     3074 2023-05-16 07:57:06.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/XmlParser/Xml.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      162 2023-05-16 08:02:55.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/XmlParser/__init__.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      405 2023-05-16 08:04:59.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/__init__.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:24:43.138650 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MySerializer/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      466 2023-05-16 07:57:06.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MySerializer/Factory.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      418 2023-05-15 21:35:45.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MySerializer/Serializer.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      134 2023-05-16 07:57:06.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/MySerializer/__init__.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:21:31.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3/__init__.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:24:43.134650 kolyaklimkLab3-4.0.0/kolyaklimkLab3.egg-info/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       93 2023-05-16 08:24:43.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3.egg-info/PKG-INFO
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      734 2023-05-16 08:24:43.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3.egg-info/SOURCES.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 08:24:43.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3.egg-info/dependency_links.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 08:24:43.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3.egg-info/not-zip-safe
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       15 2023-05-16 08:24:43.000000 kolyaklimkLab3-4.0.0/kolyaklimkLab3.egg-info/top_level.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       38 2023-05-16 08:24:43.138650 kolyaklimkLab3-4.0.0/setup.cfg
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      399 2023-05-16 08:24:41.000000 kolyaklimkLab3-4.0.0/setup.py
```

### Comparing `kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/Constants.py` & `kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/Constants.py`

 * *Files identical despite different names*

### Comparing `kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/JsonParser/Constants.py` & `kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/JsonParser/Constants.py`

 * *Files identical despite different names*

### Comparing `kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/JsonParser/Json.py` & `kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/JsonParser/Json.py`

 * *Files identical despite different names*

### Comparing `kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/Parser.py` & `kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/Parser.py`

 * *Files identical despite different names*

### Comparing `kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/XmlParser/Constants.py` & `kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/XmlParser/Constants.py`

 * *Files identical despite different names*

### Comparing `kolyaklimkLab3-3.0.0/kolyaklimkLab3/MyParser/XmlParser/Xml.py` & `kolyaklimkLab3-4.0.0/kolyaklimkLab3/MyParser/XmlParser/Xml.py`

 * *Files identical despite different names*

### Comparing `kolyaklimkLab3-3.0.0/kolyaklimkLab3.egg-info/SOURCES.txt` & `kolyaklimkLab3-4.0.0/kolyaklimkLab3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

