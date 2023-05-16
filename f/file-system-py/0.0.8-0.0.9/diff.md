# Comparing `tmp/file_system_py-0.0.8.tar.gz` & `tmp/file_system_py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_system_py-0.0.8.tar", last modified: Sat Nov 19 16:49:39 2022, max compression
+gzip compressed data, was "file_system_py-0.0.9.tar", last modified: Sat Nov 19 17:03:31 2022, max compression
```

## Comparing `file_system_py-0.0.8.tar` & `file_system_py-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-19 16:49:39.140257 file_system_py-0.0.8/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2153 2022-11-19 16:49:39.140117 file_system_py-0.0.8/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-19 16:49:39.139249 file_system_py-0.0.8/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    10699 2022-11-19 15:42:33.000000 file_system_py-0.0.8/file_system_py/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-19 16:49:39.139928 file_system_py-0.0.8/file_system_py.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2153 2022-11-19 16:49:38.000000 file_system_py-0.0.8/file_system_py.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      187 2022-11-19 16:49:39.000000 file_system_py-0.0.8/file_system_py.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-11-19 16:49:38.000000 file_system_py-0.0.8/file_system_py.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       15 2022-11-19 16:49:39.000000 file_system_py-0.0.8/file_system_py.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-11-19 16:49:39.140302 file_system_py-0.0.8/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2022-10-21 13:38:58.000000 file_system_py-0.0.8/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-19 17:03:31.116176 file_system_py-0.0.9/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2153 2022-11-19 17:03:31.116025 file_system_py-0.0.9/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-19 17:03:31.115279 file_system_py-0.0.9/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    10758 2022-11-19 17:01:46.000000 file_system_py-0.0.9/file_system_py/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-11-19 17:03:31.115838 file_system_py-0.0.9/file_system_py.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2153 2022-11-19 17:03:30.000000 file_system_py-0.0.9/file_system_py.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      187 2022-11-19 17:03:31.000000 file_system_py-0.0.9/file_system_py.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-11-19 17:03:30.000000 file_system_py-0.0.9/file_system_py.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       15 2022-11-19 17:03:30.000000 file_system_py-0.0.9/file_system_py.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-11-19 17:03:31.116218 file_system_py-0.0.9/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2022-10-21 13:38:58.000000 file_system_py-0.0.9/setup.py
```

### Comparing `file_system_py-0.0.8/PKG-INFO` & `file_system_py-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_system_py
-Version: 0.0.8
+Version: 0.0.9
 Summary: All-in-one file manipulation
 Home-page: https://github.com/jeff-hykin/file-system-py
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `file_system_py-0.0.8/file_system_py/__init__.py` & `file_system_py-0.0.9/file_system_py/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,20 +250,22 @@
 def extname(path):
     filename, file_extension = os.path.splitext(path)
     return file_extension
 
 def without_ext(path):
     started_with_dot_slash = path.startswith("./")
     parent_folders = os.path.dirname(path)
-    filename, file_extension = os.path.splitext(path)
+    filename, file_extension = os.path.splitext(os.path.basename(path))
     output = os.path.join(parent_folders, filename)
     if not started_with_dot_slash and output.startswith("./"):
         output = output[2:]
     return output
 
+without_extension = without_ext # alias
+
 def path_pieces(path):
     """
     example:
         *folders, file_name, file_extension = path_pieces("/this/is/a/filepath.txt")
     """
     folders = []
     while 1:
```

### Comparing `file_system_py-0.0.8/file_system_py.egg-info/PKG-INFO` & `file_system_py-0.0.9/file_system_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-system-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: All-in-one file manipulation
 Home-page: https://github.com/jeff-hykin/file-system-py
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `file_system_py-0.0.8/setup.py` & `file_system_py-0.0.9/setup.py`

 * *Files identical despite different names*

