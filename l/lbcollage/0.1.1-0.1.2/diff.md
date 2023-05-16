# Comparing `tmp/lbcollage-0.1.1.tar.gz` & `tmp/lbcollage-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbcollage-0.1.1.tar", last modified: Mon May 15 15:16:12 2023, max compression
+gzip compressed data, was "lbcollage-0.1.2.tar", last modified: Tue May 16 09:34:41 2023, max compression
```

## Comparing `lbcollage-0.1.1.tar` & `lbcollage-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 15:16:12.969017 lbcollage-0.1.1/
--rw-rw-rw-   0        0        0      196 2023-05-15 15:16:12.969017 lbcollage-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-05-15 15:15:24.000000 lbcollage-0.1.1/README.md
--rw-rw-rw-   0        0        0      379 2023-05-15 15:15:57.000000 lbcollage-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 15:16:12.969017 lbcollage-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 15:16:12.948901 lbcollage-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 15:16:12.960997 lbcollage-0.1.1/src/lbcollage/
--rw-rw-rw-   0        0        0      669 2023-05-15 14:59:36.000000 lbcollage-0.1.1/src/lbcollage/__init__.py
--rw-rw-rw-   0        0        0     1599 2023-05-15 14:55:28.000000 lbcollage-0.1.1/src/lbcollage/brainzrequest.py
--rw-rw-rw-   0        0        0       18 2023-05-15 14:54:48.000000 lbcollage-0.1.1/src/lbcollage/constants.py
--rw-rw-rw-   0        0        0     2511 2023-05-15 14:56:08.000000 lbcollage-0.1.1/src/lbcollage/imageprocessing.py
--rw-rw-rw-   0        0        0     1875 2023-05-15 14:57:23.000000 lbcollage-0.1.1/src/lbcollage/preferences.py
-drwxrwxrwx   0        0        0        0 2023-05-15 15:16:12.969017 lbcollage-0.1.1/src/lbcollage.egg-info/
--rw-rw-rw-   0        0        0      196 2023-05-15 15:16:12.000000 lbcollage-0.1.1/src/lbcollage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-05-15 15:16:12.000000 lbcollage-0.1.1/src/lbcollage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 15:16:12.000000 lbcollage-0.1.1/src/lbcollage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-15 15:16:12.000000 lbcollage-0.1.1/src/lbcollage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       46 2023-05-15 15:16:12.000000 lbcollage-0.1.1/src/lbcollage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 15:16:12.000000 lbcollage-0.1.1/src/lbcollage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 09:34:41.516127 lbcollage-0.1.2/
+-rw-rw-rw-   0        0        0     1235 2023-05-16 09:34:41.516127 lbcollage-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      996 2023-05-16 09:31:07.000000 lbcollage-0.1.2/README.md
+-rw-rw-rw-   0        0        0      403 2023-05-16 09:33:43.000000 lbcollage-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 09:34:41.516127 lbcollage-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 09:34:41.500462 lbcollage-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 09:34:41.500462 lbcollage-0.1.2/src/lbcollage/
+-rw-rw-rw-   0        0        0      669 2023-05-15 14:59:36.000000 lbcollage-0.1.2/src/lbcollage/__init__.py
+-rw-rw-rw-   0        0        0     1599 2023-05-15 14:55:28.000000 lbcollage-0.1.2/src/lbcollage/brainzrequest.py
+-rw-rw-rw-   0        0        0       18 2023-05-15 14:54:48.000000 lbcollage-0.1.2/src/lbcollage/constants.py
+-rw-rw-rw-   0        0        0     2511 2023-05-15 14:56:08.000000 lbcollage-0.1.2/src/lbcollage/imageprocessing.py
+-rw-rw-rw-   0        0        0     1875 2023-05-15 14:57:23.000000 lbcollage-0.1.2/src/lbcollage/preferences.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:34:41.516127 lbcollage-0.1.2/src/lbcollage.egg-info/
+-rw-rw-rw-   0        0        0     1235 2023-05-16 09:34:41.000000 lbcollage-0.1.2/src/lbcollage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-05-16 09:34:41.000000 lbcollage-0.1.2/src/lbcollage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 09:34:41.000000 lbcollage-0.1.2/src/lbcollage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-16 09:34:41.000000 lbcollage-0.1.2/src/lbcollage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       46 2023-05-16 09:34:41.000000 lbcollage-0.1.2/src/lbcollage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 09:34:41.000000 lbcollage-0.1.2/src/lbcollage.egg-info/top_level.txt
```

### Comparing `lbcollage-0.1.1/src/lbcollage/__init__.py` & `lbcollage-0.1.2/src/lbcollage/__init__.py`

 * *Files identical despite different names*

### Comparing `lbcollage-0.1.1/src/lbcollage/brainzrequest.py` & `lbcollage-0.1.2/src/lbcollage/brainzrequest.py`

 * *Files identical despite different names*

### Comparing `lbcollage-0.1.1/src/lbcollage/imageprocessing.py` & `lbcollage-0.1.2/src/lbcollage/imageprocessing.py`

 * *Files identical despite different names*

### Comparing `lbcollage-0.1.1/src/lbcollage/preferences.py` & `lbcollage-0.1.2/src/lbcollage/preferences.py`

 * *Files identical despite different names*

