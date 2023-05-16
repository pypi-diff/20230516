# Comparing `tmp/cakesAPI-3.0.tar.gz` & `tmp/cakesAPI-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cakesAPI-3.0.tar", last modified: Tue May 16 19:13:07 2023, max compression
+gzip compressed data, was "cakesAPI-4.0.tar", last modified: Tue May 16 19:28:44 2023, max compression
```

## Comparing `cakesAPI-3.0.tar` & `cakesAPI-4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:13:07.155618 cakesAPI-3.0/
--rw-rw-rw-   0        0        0      244 2023-05-16 19:13:07.155618 cakesAPI-3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 19:13:07.134155 cakesAPI-3.0/cakesAPI/
--rw-rw-rw-   0        0        0       50 2023-05-16 19:11:20.000000 cakesAPI-3.0/cakesAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:13:07.146343 cakesAPI-3.0/cakesAPI/api/
--rw-rw-rw-   0        0        0       39 2023-05-16 17:11:42.000000 cakesAPI-3.0/cakesAPI/api/__init__.py
--rw-rw-rw-   0        0        0     1252 2023-05-16 18:49:14.000000 cakesAPI-3.0/cakesAPI/api/api_client.py
--rw-rw-rw-   0        0        0      376 2023-05-16 18:54:29.000000 cakesAPI-3.0/cakesAPI/api/api_request.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:13:07.155618 cakesAPI-3.0/cakesAPI/models/
--rw-rw-rw-   0        0        0       28 2023-05-16 17:11:42.000000 cakesAPI-3.0/cakesAPI/models/__init__.py
--rw-rw-rw-   0        0        0      414 2023-05-14 18:39:16.000000 cakesAPI-3.0/cakesAPI/models/cake.py
--rw-rw-rw-   0        0        0      856 2023-05-14 13:11:47.000000 cakesAPI-3.0/cakesAPI/models/recipe.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:13:07.146343 cakesAPI-3.0/cakesAPI.egg-info/
--rw-rw-rw-   0        0        0      244 2023-05-16 19:13:07.000000 cakesAPI-3.0/cakesAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-05-16 19:13:07.000000 cakesAPI-3.0/cakesAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:13:07.000000 cakesAPI-3.0/cakesAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 19:13:07.000000 cakesAPI-3.0/cakesAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 19:13:07.000000 cakesAPI-3.0/cakesAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 19:13:07.155618 cakesAPI-3.0/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-05-16 19:09:35.000000 cakesAPI-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:28:44.728480 cakesAPI-4.0/
+-rw-rw-rw-   0        0        0      244 2023-05-16 19:28:44.728480 cakesAPI-4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 19:28:44.706692 cakesAPI-4.0/cakesAPI/
+-rw-rw-rw-   0        0        0        0 2023-05-16 19:28:41.000000 cakesAPI-4.0/cakesAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:28:44.728480 cakesAPI-4.0/cakesAPI/api/
+-rw-rw-rw-   0        0        0        2 2023-05-16 19:28:41.000000 cakesAPI-4.0/cakesAPI/api/__init__.py
+-rw-rw-rw-   0        0        0     1252 2023-05-16 18:49:14.000000 cakesAPI-4.0/cakesAPI/api/api_client.py
+-rw-rw-rw-   0        0        0      376 2023-05-16 18:54:29.000000 cakesAPI-4.0/cakesAPI/api/api_request.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:28:44.728480 cakesAPI-4.0/cakesAPI/models/
+-rw-rw-rw-   0        0        0        2 2023-05-16 19:28:41.000000 cakesAPI-4.0/cakesAPI/models/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-05-14 18:39:16.000000 cakesAPI-4.0/cakesAPI/models/cake.py
+-rw-rw-rw-   0        0        0      856 2023-05-14 13:11:47.000000 cakesAPI-4.0/cakesAPI/models/recipe.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:28:44.727017 cakesAPI-4.0/cakesAPI.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-05-16 19:28:44.000000 cakesAPI-4.0/cakesAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-16 19:28:44.000000 cakesAPI-4.0/cakesAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 19:28:44.000000 cakesAPI-4.0/cakesAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 19:28:44.000000 cakesAPI-4.0/cakesAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 19:28:44.000000 cakesAPI-4.0/cakesAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 19:28:44.728480 cakesAPI-4.0/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-05-16 19:28:41.000000 cakesAPI-4.0/setup.py
```

### Comparing `cakesAPI-3.0/cakesAPI/api/api_client.py` & `cakesAPI-4.0/cakesAPI/api/api_client.py`

 * *Files identical despite different names*

### Comparing `cakesAPI-3.0/cakesAPI/models/recipe.py` & `cakesAPI-4.0/cakesAPI/models/recipe.py`

 * *Files identical despite different names*

