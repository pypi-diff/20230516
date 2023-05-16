# Comparing `tmp/tamarind-0.2.0.tar.gz` & `tmp/tamarind-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tamarind-0.2.0.tar", last modified: Fri Jan 22 17:13:42 2021, max compression
+gzip compressed data, was "tamarind-0.2.1.tar", last modified: Tue May 16 13:48:27 2023, max compression
```

## Comparing `tamarind-0.2.0.tar` & `tamarind-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-01-22 17:13:42.000000 tamarind-0.2.0/
--rw-r--r--   0 mateljk1   (501) staff       (20)     4262 2021-01-22 17:13:42.000000 tamarind-0.2.0/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)     2977 2021-01-22 17:13:01.000000 tamarind-0.2.0/README.md
--rw-r--r--   0 mateljk1   (501) staff       (20)       38 2021-01-22 17:13:42.000000 tamarind-0.2.0/setup.cfg
--rw-r--r--   0 mateljk1   (501) staff       (20)     2753 2021-01-22 17:13:01.000000 tamarind-0.2.0/setup.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-01-22 17:13:42.000000 tamarind-0.2.0/tamarind/
--rw-r--r--   0 mateljk1   (501) staff       (20)     9137 2021-01-22 17:13:01.000000 tamarind-0.2.0/tamarind/__init__.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-01-22 17:13:42.000000 tamarind-0.2.0/tamarind.egg-info/
--rw-r--r--   0 mateljk1   (501) staff       (20)     4262 2021-01-22 17:13:41.000000 tamarind-0.2.0/tamarind.egg-info/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)      198 2021-01-22 17:13:41.000000 tamarind-0.2.0/tamarind.egg-info/SOURCES.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)        1 2021-01-22 17:13:41.000000 tamarind-0.2.0/tamarind.egg-info/dependency_links.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)       52 2021-01-22 17:13:41.000000 tamarind-0.2.0/tamarind.egg-info/requires.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)        9 2021-01-22 17:13:41.000000 tamarind-0.2.0/tamarind.egg-info/top_level.txt
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-05-16 13:48:27.715991 tamarind-0.2.1/
+-rw-r--r--   0 mateljk1   (502) staff       (20)    10173 2023-05-16 13:47:53.000000 tamarind-0.2.1/LICENSE
+-rw-r--r--   0 mateljk1   (502) staff       (20)     3521 2023-05-16 13:48:27.715580 tamarind-0.2.1/PKG-INFO
+-rw-r--r--   0 mateljk1   (502) staff       (20)     2977 2023-05-16 13:47:53.000000 tamarind-0.2.1/README.md
+-rw-r--r--   0 mateljk1   (502) staff       (20)       38 2023-05-16 13:48:27.716139 tamarind-0.2.1/setup.cfg
+-rw-r--r--   0 mateljk1   (502) staff       (20)     2736 2023-05-16 13:48:17.000000 tamarind-0.2.1/setup.py
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-05-16 13:48:27.711988 tamarind-0.2.1/tamarind/
+-rw-r--r--   0 mateljk1   (502) staff       (20)     9137 2023-05-16 13:47:53.000000 tamarind-0.2.1/tamarind/__init__.py
+drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2023-05-16 13:48:27.714887 tamarind-0.2.1/tamarind.egg-info/
+-rw-r--r--   0 mateljk1   (502) staff       (20)     3521 2023-05-16 13:48:27.000000 tamarind-0.2.1/tamarind.egg-info/PKG-INFO
+-rw-r--r--   0 mateljk1   (502) staff       (20)      206 2023-05-16 13:48:27.000000 tamarind-0.2.1/tamarind.egg-info/SOURCES.txt
+-rw-r--r--   0 mateljk1   (502) staff       (20)        1 2023-05-16 13:48:27.000000 tamarind-0.2.1/tamarind.egg-info/dependency_links.txt
+-rw-r--r--   0 mateljk1   (502) staff       (20)       35 2023-05-16 13:48:27.000000 tamarind-0.2.1/tamarind.egg-info/requires.txt
+-rw-r--r--   0 mateljk1   (502) staff       (20)        9 2023-05-16 13:48:27.000000 tamarind-0.2.1/tamarind.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tamarind-0.2.0/README.md` & `tamarind-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tamarind-0.2.0/setup.py` & `tamarind-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 # Package meta-data.
 NAME = "tamarind"
 DESCRIPTION = "More Neo4j than you can shake a cat at"
 URL = "https://github.com/FitMango/tamarind"
 EMAIL = "opensource@fitmango.com"
 AUTHOR = "Jordan Matelsky"
-REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.2.0"
+REQUIRES_PYTHON = ">=3.9.0"
+VERSION = "0.2.1"
 
 # What packages are required for this module to be executed?
-REQUIRED = ["py2neo==2020.1.1", "docker==4.4.1"]
+REQUIRED = ["py2neo", "docker"]
 
 # What packages are suggested for doing development?
 DEVELOPING_REQS = ["pytest", "pylint"]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
```

### Comparing `tamarind-0.2.0/tamarind/__init__.py` & `tamarind-0.2.1/tamarind/__init__.py`

 * *Files identical despite different names*

