# Comparing `tmp/hifi-2.0.0-py3.9.egg` & `tmp/hifi-3.0.0-py3.9.egg`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5885 bytes, number of entries: 8
--rw-r--r--  2.0 unx     5145 b- defN 23-May-15 18:24 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      207 b- defN 23-May-15 18:24 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:24 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx     1519 b- defN 23-May-15 18:24 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:24 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:24 EGG-INFO/zip-safe
--rwxr-xr-x  2.0 unx     3192 b- defN 23-May-15 18:24 EGG-INFO/scripts/hifi
--rwxr-xr-x  2.0 unx     1543 b- defN 23-May-15 18:24 EGG-INFO/scripts/visbeats
-8 files, 11609 bytes uncompressed, 4911 bytes compressed:  57.7%
+Zip file size: 5888 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     5145 b- defN 23-May-15 18:31 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      207 b- defN 23-May-15 18:31 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:31 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx     1519 b- defN 23-May-15 18:31 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:31 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:31 EGG-INFO/zip-safe
+-rwxr-xr-x  2.0 unx     3192 b- defN 23-May-15 18:31 EGG-INFO/scripts/hifi
+-rwxr-xr-x  2.0 unx     1552 b- defN 23-May-15 18:31 EGG-INFO/scripts/visbeats
+8 files, 11618 bytes uncompressed, 4914 bytes compressed:  57.7%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hifi
-Version: 2.0.0
+Version: 3.0.0
 Summary: Command-line tool to find nearest store.
 Home-page: https://github.com/austinbrown34/hifi
 Author: Austin Brown
 Author-email: austinbrown34@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## EGG-INFO/scripts/visbeats

```diff
@@ -1,14 +1,14 @@
 #!/Users/austinbrown/.local/share/virtualenvs/hifi-xpvT5RK6/bin/python
 
 import sys
 import argparse
 import matplotlib
 matplotlib.use('PS')
-import hifi.visbeats as visbeats
+import hifi.visbeats.visbeats as visbeats
 import os
 
 
 def main(args):
     print("args: {}".format(args))
 
     source_url = args.source
```

