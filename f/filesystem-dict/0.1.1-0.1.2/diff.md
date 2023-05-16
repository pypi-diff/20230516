# Comparing `tmp/filesystem-dict-0.1.1.tar.gz` & `tmp/filesystem-dict-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filesystem-dict-0.1.1.tar", last modified: Mon May 15 21:45:08 2023, max compression
+gzip compressed data, was "filesystem-dict-0.1.2.tar", last modified: Tue May 16 08:18:16 2023, max compression
```

## Comparing `filesystem-dict-0.1.1.tar` & `filesystem-dict-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 21:45:08.708768 filesystem-dict-0.1.1/
--rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-15 20:22:54.000000 filesystem-dict-0.1.1/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)      855 2023-05-15 21:45:08.708768 filesystem-dict-0.1.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      540 2023-05-15 20:56:08.000000 filesystem-dict-0.1.1/README.md
--rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-15 21:45:08.708768 filesystem-dict-0.1.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-15 20:55:49.000000 filesystem-dict-0.1.1/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 21:45:08.705434 filesystem-dict-0.1.1/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 21:45:08.705434 filesystem-dict-0.1.1/src/filesystem_dict.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      855 2023-05-15 21:45:08.000000 filesystem-dict-0.1.1/src/filesystem_dict.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-15 21:45:08.000000 filesystem-dict-0.1.1/src/filesystem_dict.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-15 21:45:08.000000 filesystem-dict-0.1.1/src/filesystem_dict.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-15 21:45:08.000000 filesystem-dict-0.1.1/src/filesystem_dict.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-15 21:45:08.708768 filesystem-dict-0.1.1/src/fsdict/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-15 20:53:38.000000 filesystem-dict-0.1.1/src/fsdict/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2195 2023-05-15 21:44:33.000000 filesystem-dict-0.1.1/src/fsdict/fsdict.py
--rw-r--r--   0 user      (1000) user      (1000)      836 2023-05-15 21:00:35.000000 filesystem-dict-0.1.1/src/fsdict/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 08:18:16.017614 filesystem-dict-0.1.2/
+-rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-15 20:22:54.000000 filesystem-dict-0.1.2/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)      855 2023-05-16 08:18:16.017614 filesystem-dict-0.1.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      540 2023-05-15 20:56:08.000000 filesystem-dict-0.1.2/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-16 08:18:16.020947 filesystem-dict-0.1.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-15 20:55:49.000000 filesystem-dict-0.1.2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 08:18:16.017614 filesystem-dict-0.1.2/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 08:18:16.017614 filesystem-dict-0.1.2/src/filesystem_dict.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      855 2023-05-16 08:18:16.000000 filesystem-dict-0.1.2/src/filesystem_dict.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-16 08:18:16.000000 filesystem-dict-0.1.2/src/filesystem_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-16 08:18:16.000000 filesystem-dict-0.1.2/src/filesystem_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-16 08:18:16.000000 filesystem-dict-0.1.2/src/filesystem_dict.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 08:18:16.017614 filesystem-dict-0.1.2/src/fsdict/
+-rw-r--r--   0 user      (1000) user      (1000)       27 2023-05-16 07:52:47.000000 filesystem-dict-0.1.2/src/fsdict/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3172 2023-05-16 08:16:59.000000 filesystem-dict-0.1.2/src/fsdict/fsdict.py
+-rw-r--r--   0 user      (1000) user      (1000)     1116 2023-05-16 08:07:12.000000 filesystem-dict-0.1.2/src/fsdict/utils.py
```

### Comparing `filesystem-dict-0.1.1/LICENSE.txt` & `filesystem-dict-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.1/PKG-INFO` & `filesystem-dict-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
```

### Comparing `filesystem-dict-0.1.1/README.md` & `filesystem-dict-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.1/src/filesystem_dict.egg-info/PKG-INFO` & `filesystem-dict-0.1.2/src/filesystem_dict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
```

### Comparing `filesystem-dict-0.1.1/src/fsdict/fsdict.py` & `filesystem-dict-0.1.2/src/fsdict/fsdict.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,111 @@
 import json
 from fsdict.utils import *
 from pathlib import Path
 
 
 class fsdict:
-    def __init__(self, path):
-        self.path = Path(path)
+    def __init__(self, path=None):
+        self.path = Path(path) if path else None
+        if self.path != None:
+            if not self.path.exists():
+                self.path.mkdir()
+            assert self.path.is_dir()
 
     def __getitem__(self, key):
+        assert not self.dangling()
         if not self.has_key(key):
             raise KeyError(key)
         key_path = self.__get_keypath(key)
         if self.__is_fsdict(key):
             return fsdict(key_path)
         else:
             return maybe_deserialize(fread_bytes(key_path))
 
     def __setitem__(self, key, value):
+        assert not self.dangling()
         key_path = self.__get_keypath(key)
+        if key_path.exists():
+            rm(key_path)
         if isinstance(value, fsdict):
-            value.copy(key_path)
+            if value.dangling():
+                key_path.mkdir()
+            else:
+                value.copy(key_path)
         else:
             fwrite_bytes(key_path, maybe_serialize(value))
 
+    def __delitem__(self, key):
+        assert not self.dangling()
+        key_path = self.__get_keypath(key)
+        if key_path.exists():
+            rm(key_path)
+
     def __repr__(self):
         return json.dumps(self.todict(), indent=2)
 
+    def dangling(self):
+        return self.path == None
+
+    def setpath(self, path):
+        self.path = Path(path)
+
     def todict(self, lazy=True):
+        assert not self.dangling()
         dictionary = dict()
         for key in self.keys():
             if self.__is_fsdict(key):
                 key_path = self.__get_keypath(key)
                 dictionary[key] = fsdict(key_path).todict(lazy)
                 continue
             if lazy:
                 dictionary[key] = "<lazy>"
             else:
                 dictionary[key] = self[key]
         return dictionary
 
     def has_key(self, key):
+        assert not self.dangling()
         key_path = self.__get_keypath(key)
         return key_path.exists()
 
     def keys(self, lazy=False):
+        assert not self.dangling()
         keys = (keypath.name for keypath in self.__get_keypaths())
         if lazy:
             return keys
         else:
             return list(keys)
 
     def values(self, lazy=True):
+        assert not self.dangling()
         values = (self[key] for key in self.keys())
         if lazy:
             return values
         else:
             return list(values)
 
     def items(self):
+        assert not self.dangling()
         for key in self.keys():
             yield key, self[key]
 
     def copy(self, dst_path):
+        assert not self.dangling()
         symlink(self.path, dst_path)
 
     def __get_keypath(self, key):
+        assert not self.dangling()
         if not isinstance(key, str):
             raise TypeError(f"Value of key must be of type 'str' not '{type(key)}'")
         return self.path / key
 
     def __get_keypaths(self):
+        assert not self.dangling()
         return self.path.glob("*")
 
     def __is_fsdict(self, key):
+        assert not self.dangling()
         if not self.has_key(key):
             raise KeyError(key)
         key_path = self.path / key
         return key_path.is_dir()
```

