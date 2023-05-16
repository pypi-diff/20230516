# Comparing `tmp/sync_list-1.0.1.tar.gz` & `tmp/sync_list-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sync_list-1.0.1.tar", max compression
+gzip compressed data, was "sync_list-1.0.2.tar", max compression
```

## Comparing `sync_list-1.0.1.tar` & `sync_list-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1024 2023-05-16 00:18:04.740403 sync_list-1.0.1/README.md
--rw-r--r--   0        0        0      411 2023-05-16 00:18:04.740403 sync_list-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-16 00:18:04.740403 sync_list-1.0.1/sync_list/__init__.py
--rw-r--r--   0        0        0     1907 2023-05-16 00:18:04.740403 sync_list-1.0.1/sync_list/_sync_list_.py
--rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 sync_list-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1024 2023-05-16 17:28:45.374530 sync_list-1.0.2/README.md
+-rw-r--r--   0        0        0      412 2023-05-16 17:28:45.374530 sync_list-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-16 17:28:45.374530 sync_list-1.0.2/sync_list/__init__.py
+-rw-r--r--   0        0        0     1907 2023-05-16 17:28:45.374530 sync_list-1.0.2/sync_list/_sync_list_.py
+-rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 sync_list-1.0.2/PKG-INFO
```

### Comparing `sync_list-1.0.1/README.md` & `sync_list-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sync_list-1.0.1/sync_list/_sync_list_.py` & `sync_list-1.0.2/sync_list/_sync_list_.py`

 * *Files identical despite different names*

### Comparing `sync_list-1.0.1/PKG-INFO` & `sync_list-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sync-list
-Version: 1.0.1
+Version: 1.0.2
 Summary: SyncList - список Python с автоматической синхронизацией данных с файлом JSON.
 Author: Azreil-OFD
 Author-email: fantom2413@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

