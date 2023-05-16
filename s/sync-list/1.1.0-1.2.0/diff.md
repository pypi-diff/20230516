# Comparing `tmp/sync_list-1.1.0.tar.gz` & `tmp/sync_list-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sync_list-1.1.0.tar", max compression
+gzip compressed data, was "sync_list-1.2.0.tar", max compression
```

## Comparing `sync_list-1.1.0.tar` & `sync_list-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1024 2023-05-16 19:33:09.603421 sync_list-1.1.0/README.md
--rw-r--r--   0        0        0      412 2023-05-16 19:33:09.603421 sync_list-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-16 19:33:09.603421 sync_list-1.1.0/sync_list/__init__.py
--rw-r--r--   0        0        0     2893 2023-05-16 19:33:09.603421 sync_list-1.1.0/sync_list/_sync_list_.py
--rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 sync_list-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1024 2023-05-16 21:28:57.196677 sync_list-1.2.0/README.md
+-rw-r--r--   0        0        0      412 2023-05-16 21:28:57.196677 sync_list-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-16 21:28:57.196677 sync_list-1.2.0/sync_list/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-16 21:28:57.196677 sync_list-1.2.0/sync_list/_sync_list_.py
+-rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 sync_list-1.2.0/PKG-INFO
```

### Comparing `sync_list-1.1.0/README.md` & `sync_list-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sync_list-1.1.0/sync_list/_sync_list_.py` & `sync_list-1.2.0/sync_list/_sync_list_.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,23 @@
         return iter(self._data[self.bucket])
 
     def __reversed__(self):
         return reversed(self._data[self.bucket])
 
     def __repr__(self):
         return repr(self._data[self.bucket])
+        # Метод для сериализации в JSON
+
+    def to_json(self):
+        return json.dumps(self._data[self.bucket])
+
+    @classmethod
+    def from_json(cls, json_str, filename='data.json', bucket_name='default'):
+        items = json.loads(json_str)
+        return cls(items, filename, bucket_name)
 
     def index(self, item):
         return self._data[self.bucket].index(item)
 
     def count(self, item):
         return self._data[self.bucket].count(item)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sync_list-1.1.0/PKG-INFO` & `sync_list-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sync-list
-Version: 1.1.0
+Version: 1.2.0
 Summary: SyncList - список Python с автоматической синхронизацией данных с файлом JSON.
 Author: Azreil-OFD
 Author-email: fantom2413@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

