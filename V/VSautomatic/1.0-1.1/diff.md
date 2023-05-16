# Comparing `tmp/VSautomatic-1.0.tar.gz` & `tmp/VSautomatic-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VSautomatic-1.0.tar", last modified: Mon May 15 09:45:57 2023, max compression
+gzip compressed data, was "VSautomatic-1.1.tar", last modified: Tue May 16 03:31:55 2023, max compression
```

## Comparing `VSautomatic-1.0.tar` & `VSautomatic-1.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:45:57.049832 VSautomatic-1.0/
--rw-rw-rw-   0        0        0      259 2023-05-15 09:45:57.049832 VSautomatic-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-15 09:45:57.039833 VSautomatic-1.0/VSautomatic/
--rw-rw-rw-   0        0        0     2604 2023-05-12 09:51:44.000000 VSautomatic-1.0/VSautomatic/MyCamera.py
--rw-rw-rw-   0        0        0     1460 2023-05-15 08:57:34.000000 VSautomatic-1.0/VSautomatic/MyRedRat.py
--rw-rw-rw-   0        0        0     5228 2023-05-15 08:56:26.000000 VSautomatic-1.0/VSautomatic/MyTools.py
--rw-rw-rw-   0        0        0    18705 2023-05-15 06:00:03.000000 VSautomatic-1.0/VSautomatic/ReSTTerminal.py
--rw-rw-rw-   0        0        0     1768 2023-05-15 08:56:52.000000 VSautomatic-1.0/VSautomatic/RedRatHub.py
--rw-rw-rw-   0        0        0     1287 2023-05-15 09:15:19.000000 VSautomatic-1.0/VSautomatic/RedRatHubS.py
--rw-rw-rw-   0        0        0     2522 2023-04-11 06:19:42.000000 VSautomatic-1.0/VSautomatic/TestCfgParse.py
--rw-rw-rw-   0        0        0      154 2023-05-12 09:17:16.000000 VSautomatic-1.0/VSautomatic/__init__.py
--rw-rw-rw-   0        0        0     1121 2023-05-06 06:48:49.000000 VSautomatic-1.0/VSautomatic/deco.py
--rw-rw-rw-   0        0        0     3230 2023-05-12 08:47:07.000000 VSautomatic-1.0/VSautomatic/my_serial.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:45:57.049832 VSautomatic-1.0/VSautomatic.egg-info/
--rw-rw-rw-   0        0        0      259 2023-05-15 09:45:56.000000 VSautomatic-1.0/VSautomatic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-05-15 09:45:56.000000 VSautomatic-1.0/VSautomatic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:45:56.000000 VSautomatic-1.0/VSautomatic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 09:45:56.000000 VSautomatic-1.0/VSautomatic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 09:45:57.049832 VSautomatic-1.0/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-05-15 09:45:44.000000 VSautomatic-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:31:55.399793 VSautomatic-1.1/
+-rw-rw-rw-   0        0        0      259 2023-05-16 03:31:55.399793 VSautomatic-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 03:31:55.385270 VSautomatic-1.1/VSautomatic/
+-rw-rw-rw-   0        0        0       10 2023-05-15 06:47:27.000000 VSautomatic-1.1/VSautomatic/Auth_Token.txt
+-rw-rw-rw-   0        0        0    24737 2022-10-28 06:26:28.000000 VSautomatic-1.1/VSautomatic/Dictionary.txt
+-rw-rw-rw-   0        0        0     2604 2023-05-12 09:51:44.000000 VSautomatic-1.1/VSautomatic/MyCamera.py
+-rw-rw-rw-   0        0        0     1460 2023-05-15 08:57:34.000000 VSautomatic-1.1/VSautomatic/MyRedRat.py
+-rw-rw-rw-   0        0        0     5228 2023-05-15 08:56:26.000000 VSautomatic-1.1/VSautomatic/MyTools.py
+-rw-rw-rw-   0        0        0    18705 2023-05-15 06:00:03.000000 VSautomatic-1.1/VSautomatic/ReSTTerminal.py
+-rw-rw-rw-   0        0        0     1768 2023-05-15 08:56:52.000000 VSautomatic-1.1/VSautomatic/RedRatHub.py
+-rw-rw-rw-   0        0        0     1287 2023-05-15 09:15:19.000000 VSautomatic-1.1/VSautomatic/RedRatHubS.py
+-rw-rw-rw-   0        0        0     2522 2023-04-11 06:19:42.000000 VSautomatic-1.1/VSautomatic/TestCfgParse.py
+-rw-rw-rw-   0        0        0      154 2023-05-12 09:17:16.000000 VSautomatic-1.1/VSautomatic/__init__.py
+-rw-rw-rw-   0        0        0     1121 2023-05-06 06:48:49.000000 VSautomatic-1.1/VSautomatic/deco.py
+-rw-rw-rw-   0        0        0     3230 2023-05-12 08:47:07.000000 VSautomatic-1.1/VSautomatic/my_serial.py
+-rw-rw-rw-   0        0        0       81 2023-05-15 06:49:02.000000 VSautomatic-1.1/VSautomatic/restlog.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 03:31:55.397512 VSautomatic-1.1/VSautomatic.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-05-16 03:31:55.000000 VSautomatic-1.1/VSautomatic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-05-16 03:31:55.000000 VSautomatic-1.1/VSautomatic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 03:31:55.000000 VSautomatic-1.1/VSautomatic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 03:31:55.000000 VSautomatic-1.1/VSautomatic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 03:31:55.399793 VSautomatic-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-05-16 03:26:46.000000 VSautomatic-1.1/setup.py
```

### Comparing `VSautomatic-1.0/VSautomatic/MyCamera.py` & `VSautomatic-1.1/VSautomatic/MyCamera.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-1.0/VSautomatic/MyRedRat.py` & `VSautomatic-1.1/VSautomatic/MyRedRat.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-1.0/VSautomatic/MyTools.py` & `VSautomatic-1.1/VSautomatic/MyTools.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-1.0/VSautomatic/ReSTTerminal.py` & `VSautomatic-1.1/VSautomatic/ReSTTerminal.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-1.0/VSautomatic/RedRatHub.py` & `VSautomatic-1.1/VSautomatic/RedRatHub.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-1.0/VSautomatic/RedRatHubS.py` & `VSautomatic-1.1/VSautomatic/RedRatHubS.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-1.0/VSautomatic/TestCfgParse.py` & `VSautomatic-1.1/VSautomatic/TestCfgParse.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-1.0/VSautomatic/deco.py` & `VSautomatic-1.1/VSautomatic/deco.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-1.0/VSautomatic/my_serial.py` & `VSautomatic-1.1/VSautomatic/my_serial.py`

 * *Files identical despite different names*

