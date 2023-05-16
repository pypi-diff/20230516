# Comparing `tmp/ovos_PHAL-0.0.5a5-py3-none-any.whl.zip` & `tmp/ovos_PHAL-0.0.5a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9562 bytes, number of entries: 12
--rw-r--r--  2.0 unx      148 b- defN 23-May-12 20:32 ovos_PHAL/__init__.py
--rw-r--r--  2.0 unx      572 b- defN 23-May-12 20:32 ovos_PHAL/__main__.py
--rw-r--r--  2.0 unx     2569 b- defN 23-May-12 20:32 ovos_PHAL/admin.py
--rw-r--r--  2.0 unx     1436 b- defN 23-May-12 20:32 ovos_PHAL/detection.py
--rw-r--r--  2.0 unx     3047 b- defN 23-May-12 20:32 ovos_PHAL/service.py
--rw-r--r--  2.0 unx      177 b- defN 23-May-12 20:32 ovos_PHAL/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1384 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       94 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 23-May-12 20:32 ovos_PHAL-0.0.5a5.dist-info/RECORD
-12 files, 21845 bytes uncompressed, 7938 bytes compressed:  63.7%
+Zip file size: 9542 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      148 b- defN 23-May-16 17:47 ovos_PHAL/__init__.py
+-rw-r--r--  2.0 unx      572 b- defN 23-May-16 17:47 ovos_PHAL/__main__.py
+-rw-r--r--  2.0 unx     2569 b- defN 23-May-16 17:47 ovos_PHAL/admin.py
+-rw-r--r--  2.0 unx     1436 b- defN 23-May-16 17:47 ovos_PHAL/detection.py
+-rw-r--r--  2.0 unx     3047 b- defN 23-May-16 17:47 ovos_PHAL/service.py
+-rw-r--r--  2.0 unx      177 b- defN 23-May-16 17:47 ovos_PHAL/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-May-16 17:47 ovos_PHAL-0.0.5a6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1249 b- defN 23-May-16 17:47 ovos_PHAL-0.0.5a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-16 17:47 ovos_PHAL-0.0.5a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       94 b- defN 23-May-16 17:47 ovos_PHAL-0.0.5a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-16 17:47 ovos_PHAL-0.0.5a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 23-May-16 17:47 ovos_PHAL-0.0.5a6.dist-info/RECORD
+12 files, 21710 bytes uncompressed, 7918 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: ovos_PHAL/service.py
 Comment: 
 
 Filename: ovos_PHAL/version.py
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a5.dist-info/LICENSE
+Filename: ovos_PHAL-0.0.5a6.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a5.dist-info/METADATA
+Filename: ovos_PHAL-0.0.5a6.dist-info/METADATA
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a5.dist-info/WHEEL
+Filename: ovos_PHAL-0.0.5a6.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a5.dist-info/entry_points.txt
+Filename: ovos_PHAL-0.0.5a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a5.dist-info/top_level.txt
+Filename: ovos_PHAL-0.0.5a6.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_PHAL-0.0.5a5.dist-info/RECORD
+Filename: ovos_PHAL-0.0.5a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_PHAL/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 5
-VERSION_ALPHA = 5
+VERSION_ALPHA = 6
 # END_VERSION_BLOCK
```

## Comparing `ovos_PHAL-0.0.5a5.dist-info/LICENSE` & `ovos_PHAL-0.0.5a6.dist-info/LICENSE`

 * *Files identical despite different names*

