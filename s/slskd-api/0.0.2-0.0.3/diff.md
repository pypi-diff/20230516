# Comparing `tmp/slskd-api-0.0.2.tar.gz` & `tmp/slskd-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slskd-api-0.0.2.tar", last modified: Tue May 16 21:46:03 2023, max compression
+gzip compressed data, was "slskd-api-0.0.3.tar", last modified: Tue May 16 21:53:24 2023, max compression
```

## Comparing `slskd-api-0.0.2.tar` & `slskd-api-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:03.869286 slskd-api-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-16 21:46:03.869286 slskd-api-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-16 21:45:44.000000 slskd-api-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:46:03.869286 slskd-api-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 21:45:44.000000 slskd-api-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:03.865286 slskd-api-0.0.2/slskd_api/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:03.869286 slskd-api-0.0.2/slskd_api/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/conversations.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/rooms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/searches.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/shares.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/apis/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-16 21:45:44.000000 slskd-api-0.0.2/slskd_api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:03.869286 slskd-api-0.0.2/slskd_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-16 21:46:03.000000 slskd-api-0.0.2/slskd_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-16 21:46:03.000000 slskd-api-0.0.2/slskd_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:46:03.000000 slskd-api-0.0.2/slskd_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 21:46:03.000000 slskd-api-0.0.2/slskd_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 21:46:03.000000 slskd-api-0.0.2/slskd_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.864639 slskd-api-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 21:53:24.864639 slskd-api-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-16 21:53:08.000000 slskd-api-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:53:24.864639 slskd-api-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-16 21:53:08.000000 slskd-api-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.860639 slskd-api-0.0.3/slskd_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.864639 slskd-api-0.0.3/slskd_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/conversations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/shares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/apis/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-16 21:53:08.000000 slskd-api-0.0.3/slskd_api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.860639 slskd-api-0.0.3/slskd_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 21:53:24.000000 slskd-api-0.0.3/slskd_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-16 21:53:24.000000 slskd-api-0.0.3/slskd_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:53:24.000000 slskd-api-0.0.3/slskd_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 21:53:24.000000 slskd-api-0.0.3/slskd_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 21:53:24.000000 slskd-api-0.0.3/slskd_api.egg-info/top_level.txt
```

### Comparing `slskd-api-0.0.2/PKG-INFO` & `slskd-api-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: slskd-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: API Wrapper to interact with slskd
 Author: bigoulours
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 
 # slskd-api
 
 ## Goal
 This project aims at providing a python API for [slskd](https://github.com/slskd/slskd).
 
 A comprehensive python API could help improve integration and increase slskd adoption by enabling rapid development of various software, like:
```

### Comparing `slskd-api-0.0.2/README.md` & `slskd-api-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/__init__.py` & `slskd-api-0.0.3/slskd_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/application.py` & `slskd-api-0.0.3/slskd_api/apis/application.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/conversations.py` & `slskd-api-0.0.3/slskd_api/apis/conversations.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/options.py` & `slskd-api-0.0.3/slskd_api/apis/options.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/rooms.py` & `slskd-api-0.0.3/slskd_api/apis/rooms.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/searches.py` & `slskd-api-0.0.3/slskd_api/apis/searches.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/server.py` & `slskd-api-0.0.3/slskd_api/apis/server.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/session.py` & `slskd-api-0.0.3/slskd_api/apis/session.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/shares.py` & `slskd-api-0.0.3/slskd_api/apis/shares.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/transfers.py` & `slskd-api-0.0.3/slskd_api/apis/transfers.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/apis/users.py` & `slskd-api-0.0.3/slskd_api/apis/users.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api/client.py` & `slskd-api-0.0.3/slskd_api/client.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.2/slskd_api.egg-info/PKG-INFO` & `slskd-api-0.0.3/slskd_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: slskd-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: API Wrapper to interact with slskd
 Author: bigoulours
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 
 # slskd-api
 
 ## Goal
 This project aims at providing a python API for [slskd](https://github.com/slskd/slskd).
 
 A comprehensive python API could help improve integration and increase slskd adoption by enabling rapid development of various software, like:
```

### Comparing `slskd-api-0.0.2/slskd_api.egg-info/SOURCES.txt` & `slskd-api-0.0.3/slskd_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

