# Comparing `tmp/fyCursor-0.0.1.tar.gz` & `tmp/fyCursor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.0.1.tar", last modified: Sun May 14 04:40:24 2023, max compression
+gzip compressed data, was "fyCursor-0.0.2.tar", last modified: Tue May 16 02:01:07 2023, max compression
```

## Comparing `fyCursor-0.0.1.tar` & `fyCursor-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-14 04:40:24.162070 fyCursor-0.0.1/
--rw-r--r--   0 danielkay   (503) staff       (20)     1062 2023-05-14 02:45:31.000000 fyCursor-0.0.1/LICENSE
--rw-r--r--   0 danielkay   (503) staff       (20)      570 2023-05-14 04:40:24.161915 fyCursor-0.0.1/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)       59 2023-05-14 02:46:01.000000 fyCursor-0.0.1/README.md
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-14 04:40:24.159723 fyCursor-0.0.1/fyCursor/
--rw-r--r--   0 danielkay   (503) staff       (20)       24 2023-05-14 02:56:02.000000 fyCursor-0.0.1/fyCursor/__init__.py
--rw-r--r--   0 danielkay   (503) staff       (20)     4503 2023-05-14 03:29:07.000000 fyCursor-0.0.1/fyCursor/core.py
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-14 04:40:24.161695 fyCursor-0.0.1/fyCursor.egg-info/
--rw-r--r--   0 danielkay   (503) staff       (20)      570 2023-05-14 04:40:24.000000 fyCursor-0.0.1/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)      192 2023-05-14 04:40:24.000000 fyCursor-0.0.1/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        1 2023-05-14 04:40:24.000000 fyCursor-0.0.1/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        9 2023-05-14 04:40:24.000000 fyCursor-0.0.1/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 danielkay   (503) staff       (20)       38 2023-05-14 04:40:24.162126 fyCursor-0.0.1/setup.cfg
--rw-r--r--   0 danielkay   (503) staff       (20)      994 2023-05-14 04:31:34.000000 fyCursor-0.0.1/setup.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 02:01:07.470669 fyCursor-0.0.2/
+-rw-r--r--   0 danielkay   (503) staff       (20)     1062 2023-05-14 02:45:31.000000 fyCursor-0.0.2/LICENSE
+-rw-r--r--   0 danielkay   (503) staff       (20)      294 2023-05-16 02:01:07.470512 fyCursor-0.0.2/PKG-INFO
+-rw-r--r--   0 danielkay   (503) staff       (20)       59 2023-05-14 02:46:01.000000 fyCursor-0.0.2/README.md
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 02:01:07.460049 fyCursor-0.0.2/fyCursor/
+-rw-r--r--   0 danielkay   (503) staff       (20)      589 2023-05-16 01:33:40.000000 fyCursor-0.0.2/fyCursor/__init__.py
+-rw-r--r--   0 danielkay   (503) staff       (20)     4510 2023-05-16 01:30:01.000000 fyCursor-0.0.2/fyCursor/core.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 02:01:07.470123 fyCursor-0.0.2/fyCursor.egg-info/
+-rw-r--r--   0 danielkay   (503) staff       (20)      294 2023-05-16 02:01:07.000000 fyCursor-0.0.2/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 danielkay   (503) staff       (20)      192 2023-05-16 02:01:07.000000 fyCursor-0.0.2/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)        1 2023-05-16 02:01:07.000000 fyCursor-0.0.2/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)        9 2023-05-16 02:01:07.000000 fyCursor-0.0.2/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)       38 2023-05-16 02:01:07.470721 fyCursor-0.0.2/setup.cfg
+-rw-r--r--   0 danielkay   (503) staff       (20)      698 2023-05-16 01:51:46.000000 fyCursor-0.0.2/setup.py
```

### Comparing `fyCursor-0.0.1/LICENSE` & `fyCursor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.0.1/fyCursor/core.py` & `fyCursor-0.0.2/fyCursor/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     )
     return connection.cursor(fyCursor) #type: ignore
     
 
 class fyCursor(_cur):
     """
     Custom `sqlite3.Cursor` that can be used without string query. \n
-    I just hate query because it does not have any highlighting, yeah.
+    I just hate query because it does not have any highlighting in IDE, yeah.
 
     https://github.com/felixyeahh/fyCursor
     """
     def __init__(
         self, 
         __cursor: Connection, 
         logger = None
```

