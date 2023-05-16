# Comparing `tmp/panther-1.7.3.tar.gz` & `tmp/panther-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-1.7.3.tar", last modified: Fri Mar 24 20:02:55 2023, max compression
+gzip compressed data, was "panther-1.7.4.tar", last modified: Tue May 16 08:41:18 2023, max compression
```

## Comparing `panther-1.7.3.tar` & `panther-1.7.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:02:55.347879 panther-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-24 20:02:41.000000 panther-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-03-24 20:02:55.347879 panther-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-03-24 20:02:41.000000 panther-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:02:55.339879 panther-1.7.3/panther/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-24 20:02:41.000000 panther-1.7.3/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-03-24 20:02:41.000000 panther-1.7.3/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-03-24 20:02:41.000000 panther-1.7.3/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-03-24 20:02:41.000000 panther-1.7.3/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-24 20:02:41.000000 panther-1.7.3/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:02:55.343879 panther-1.7.3/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 20:02:41.000000 panther-1.7.3/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-03-24 20:02:41.000000 panther-1.7.3/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-24 20:02:41.000000 panther-1.7.3/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-24 20:02:41.000000 panther-1.7.3/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-24 20:02:41.000000 panther-1.7.3/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-24 20:02:41.000000 panther-1.7.3/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-03-24 20:02:41.000000 panther-1.7.3/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-24 20:02:41.000000 panther-1.7.3/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:02:55.347879 panther-1.7.3/panther/db/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-24 20:02:41.000000 panther-1.7.3/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-24 20:02:41.000000 panther-1.7.3/panther/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-24 20:02:41.000000 panther-1.7.3/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:02:55.347879 panther-1.7.3/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-24 20:02:41.000000 panther-1.7.3/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-24 20:02:41.000000 panther-1.7.3/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-24 20:02:41.000000 panther-1.7.3/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-03-24 20:02:41.000000 panther-1.7.3/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-24 20:02:41.000000 panther-1.7.3/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-24 20:02:41.000000 panther-1.7.3/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-03-24 20:02:41.000000 panther-1.7.3/panther/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-03-24 20:02:41.000000 panther-1.7.3/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:02:55.347879 panther-1.7.3/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 20:02:41.000000 panther-1.7.3/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-24 20:02:41.000000 panther-1.7.3/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-24 20:02:41.000000 panther-1.7.3/panther/middlewares/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-24 20:02:41.000000 panther-1.7.3/panther/middlewares/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-24 20:02:41.000000 panther-1.7.3/panther/middlewares/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-24 20:02:41.000000 panther-1.7.3/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-03-24 20:02:41.000000 panther-1.7.3/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-24 20:02:41.000000 panther-1.7.3/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-03-24 20:02:41.000000 panther-1.7.3/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-24 20:02:41.000000 panther-1.7.3/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-24 20:02:41.000000 panther-1.7.3/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-24 20:02:41.000000 panther-1.7.3/panther/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:02:55.343879 panther-1.7.3/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-03-24 20:02:55.000000 panther-1.7.3/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-24 20:02:55.000000 panther-1.7.3/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 20:02:55.000000 panther-1.7.3/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-24 20:02:55.000000 panther-1.7.3/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-24 20:02:55.000000 panther-1.7.3/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-24 20:02:55.000000 panther-1.7.3/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-24 20:02:41.000000 panther-1.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 20:02:55.347879 panther-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-24 20:02:41.000000 panther-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:18.909647 panther-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-16 08:41:01.000000 panther-1.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-16 08:41:18.909647 panther-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-16 08:41:01.000000 panther-1.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:18.905647 panther-1.7.4/panther/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 08:41:01.000000 panther-1.7.4/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-16 08:41:01.000000 panther-1.7.4/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-16 08:41:01.000000 panther-1.7.4/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-16 08:41:01.000000 panther-1.7.4/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-16 08:41:01.000000 panther-1.7.4/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:18.905647 panther-1.7.4/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.000000 panther-1.7.4/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-16 08:41:01.000000 panther-1.7.4/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-16 08:41:01.000000 panther-1.7.4/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-16 08:41:01.000000 panther-1.7.4/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-16 08:41:01.000000 panther-1.7.4/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-16 08:41:01.000000 panther-1.7.4/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-16 08:41:01.000000 panther-1.7.4/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 08:41:01.000000 panther-1.7.4/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:18.905647 panther-1.7.4/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 08:41:01.000000 panther-1.7.4/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-16 08:41:01.000000 panther-1.7.4/panther/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-16 08:41:01.000000 panther-1.7.4/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:18.909647 panther-1.7.4/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 08:41:01.000000 panther-1.7.4/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-16 08:41:01.000000 panther-1.7.4/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-16 08:41:01.000000 panther-1.7.4/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-16 08:41:01.000000 panther-1.7.4/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-16 08:41:01.000000 panther-1.7.4/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 08:41:01.000000 panther-1.7.4/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-16 08:41:01.000000 panther-1.7.4/panther/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-05-16 08:41:01.000000 panther-1.7.4/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:18.909647 panther-1.7.4/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 08:41:01.000000 panther-1.7.4/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 08:41:01.000000 panther-1.7.4/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 08:41:01.000000 panther-1.7.4/panther/middlewares/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-16 08:41:01.000000 panther-1.7.4/panther/middlewares/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-16 08:41:01.000000 panther-1.7.4/panther/middlewares/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 08:41:01.000000 panther-1.7.4/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-16 08:41:01.000000 panther-1.7.4/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-16 08:41:01.000000 panther-1.7.4/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-16 08:41:01.000000 panther-1.7.4/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-16 08:41:01.000000 panther-1.7.4/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-16 08:41:01.000000 panther-1.7.4/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-16 08:41:01.000000 panther-1.7.4/panther/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:18.905647 panther-1.7.4/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-16 08:41:18.000000 panther-1.7.4/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 08:41:18.000000 panther-1.7.4/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:41:18.000000 panther-1.7.4/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 08:41:18.000000 panther-1.7.4/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-16 08:41:18.000000 panther-1.7.4/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 08:41:18.000000 panther-1.7.4/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-16 08:41:01.000000 panther-1.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:41:18.909647 panther-1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-16 08:41:01.000000 panther-1.7.4/setup.py
```

### Comparing `panther-1.7.3/LICENSE` & `panther-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/PKG-INFO` & `panther-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.3
+Version: 1.7.4
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE
 
 ## Panther 
-<b>Is A Fast &  Friendly, Web Framework For Building Async APIs With Python 3.11+</b> 
+<b>Is A Fast &  Friendly Web Framework For Building Async APIs With Python 3.11+</b> 
 
 <p align="center">
 <img src="https://github.com/AliRn76/panther/raw/master/docs/docs/images/logo.png" alt="logo" style="width: 200px">
 </p>
 
 >_Full Documentation_ -> [https://pantherpy.github.io](https://pantherpy.github.io)
 >
```

### Comparing `panther-1.7.3/README.md` & `panther-1.7.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## Panther 
-<b>Is A Fast &  Friendly, Web Framework For Building Async APIs With Python 3.11+</b> 
+<b>Is A Fast &  Friendly Web Framework For Building Async APIs With Python 3.11+</b> 
 
 <p align="center">
 <img src="https://github.com/AliRn76/panther/raw/master/docs/docs/images/logo.png" alt="logo" style="width: 200px">
 </p>
 
 >_Full Documentation_ -> [https://pantherpy.github.io](https://pantherpy.github.io)
 >
```

### Comparing `panther-1.7.3/panther/_utils.py` & `panther-1.7.4/panther/_utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/app.py` & `panther-1.7.4/panther/app.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/authentications.py` & `panther-1.7.4/panther/authentications.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/caching.py` & `panther-1.7.4/panther/caching.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/cli/create_command.py` & `panther-1.7.4/panther/cli/create_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/cli/main.py` & `panther-1.7.4/panther/cli/main.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/cli/monitor_command.py` & `panther-1.7.4/panther/cli/monitor_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/cli/run_command.py` & `panther-1.7.4/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/cli/template.py` & `panther-1.7.4/panther/cli/template.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/cli/utils.py` & `panther-1.7.4/panther/cli/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/configs.py` & `panther-1.7.4/panther/configs.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/db/connection.py` & `panther-1.7.4/panther/db/connection.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/db/models.py` & `panther-1.7.4/panther/db/models.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/db/queries/mongodb_queries.py` & `panther-1.7.4/panther/db/queries/mongodb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/db/queries/pantherdb_queries.py` & `panther-1.7.4/panther/db/queries/pantherdb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/db/queries/queries.py` & `panther-1.7.4/panther/db/queries/queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/db/utils.py` & `panther-1.7.4/panther/db/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/exceptions.py` & `panther-1.7.4/panther/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/logger.py` & `panther-1.7.4/panther/logger.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/main.py` & `panther-1.7.4/panther/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,96 @@
 
 
 class Panther:
 
     def __init__(self, name):
         import os
         os.system('clear')
-        self.base_dir = Path(name).resolve().parent
-        config['base_dir'] = self.base_dir
-        self.panther_dir = Path(__file__).parent
+        config['base_dir'] = Path(name).resolve().parent
         self.load_configs()
         del os
 
+    def load_configs(self) -> None:
+        from panther.logger import logger
+        logger.debug(f'Base directory: {config["base_dir"]}')
+
+        # Check & Read The Configs File
+        self._check_configs()
+
+        # Put Variables In "config"
+        config['monitoring'] = self.settings.get('MONITORING', config['monitoring'])
+        config['log_queries'] = self.settings.get('LOG_QUERIES', config['log_queries'])
+        config['default_cache_exp'] = self.settings.get('DEFAULT_CACHE_EXP', config['default_cache_exp'])
+        config['throttling'] = self.settings.get('THROTTLING', config['throttling'])
+        config['secret_key'] = self._get_secret_key()
+
+        config['middlewares'] = self._get_middlewares()
+        config['reversed_middlewares'] = config['middlewares'][::-1]
+        config['user_model'] = self._get_user_model()
+
+        config['authentication'] = self._get_authentication_class()
+        config['jwt_config'] = self._get_jwt_config()
+
+        # Check & Collect URLs
+        #   check_urls should be the last call in load_configs,
+        #   because it will read all files and load them.
+        config['urls'] = self._load_urls()
+
+        logger.debug('Configs loaded.')
+        if config['monitoring']:
+            logger.info('Run "panther monitor" in another session for Monitoring.')
+
+    def _load_urls(self) -> dict:
+        urls = check_urls(self.settings.get('URLs')) or {}
+        collect_urls('', urls, collected_urls := dict())
+        return finalize_urls(collected_urls)
+
+    def _check_configs(self):
+        from panther.logger import logger
+        """Read the config file and put it as dict in self.settings"""
+        try:
+            configs_path = config['base_dir'] / 'core/configs.py'
+            self.settings = run_path(str(configs_path))
+        except FileNotFoundError:
+            logger.critical('core/configs.py Not Found.')
+
+    def _get_secret_key(self) -> bytes | None:
+        if secret_key := self.settings.get('SECRET_KEY'):
+            return secret_key.encode()
+        return secret_key
+
+    def _get_middlewares(self) -> list:
+        """Collect The Middlewares & Set db_engine If One Of Middlewares Was For DB"""
+        from panther.logger import logger
+        middlewares = list()
+
+        for path, data in self.settings.get('MIDDLEWARES', []):
+            if path.find('panther.middlewares.db.Middleware') != -1:
+                config['db_engine'] = data['url'].split(':')[0]
+
+            Middleware = import_class(path)  # NOQA: Py Pep8 Naming
+            if not issubclass(Middleware, BaseMiddleware):
+                logger.critical(f'{Middleware} is not a sub class of BaseMiddleware.')
+                continue
+
+            middlewares.append(Middleware(**data))  # NOQA: Py Argument List
+        return middlewares
+
+    def _get_authentication_class(self) -> ModelMetaclass | None:
+        return self.settings.get('AUTHENTICATION') and import_class(self.settings['AUTHENTICATION'])
+
+    def _get_user_model(self) -> ModelMetaclass:
+        return import_class(self.settings.get('USER_MODEL', 'panther.db.models.User'))
+
+    def _get_jwt_config(self) -> JWTConfig:
+        """Only Collect JWT Config If Authentication Is JWTAuthentication"""
+        if getattr(config['authentication'], '__name__', None) == 'JWTAuthentication':
+            user_config = self.settings.get('JWTConfig')
+            return JWTConfig(**user_config) if user_config else JWTConfig(key=config['secret_key'].decode())
+
     async def __call__(self, scope, receive, send) -> None:
         """
         We Used Python3.11 For asyncio.TaskGroup()
         1.
             async with asyncio.TaskGroup() as tg:
                 tg.create_task(self.run(scope, receive, send))
         2.
@@ -109,81 +185,7 @@
 
     @classmethod
     def handle_exceptions(cls, e, /) -> Response:
         return Response(
             data=e.detail if isinstance(e.detail, dict) else {'detail': e.detail},
             status_code=e.status_code,
         )
-
-    def load_configs(self) -> None:
-        from panther.logger import logger
-        logger.debug(f'Base directory: {self.base_dir}')
-
-        # Check & Read The Configs File
-        self._check_configs()
-
-        # Put Variables In "config"
-        config['monitoring'] = self.settings.get('MONITORING', config['monitoring'])
-        config['log_queries'] = self.settings.get('LOG_QUERIES', config['log_queries'])
-        config['default_cache_exp'] = self.settings.get('DEFAULT_CACHE_EXP', config['default_cache_exp'])
-        config['throttling'] = self.settings.get('THROTTLING', config['throttling'])
-        config['secret_key'] = self._get_secret_key()
-
-        config['middlewares'] = self._get_middlewares()
-        config['reversed_middlewares'] = config['middlewares'][::-1]
-        config['user_model'] = self._get_user_model()
-
-        config['authentication'] = self._get_authentication_class()
-        config['jwt_config'] = self._get_jwt_config()
-
-        # Check & Collect URLs
-        #   check_urls should be the last call in load_configs, because it will read all files and load them.
-        urls = check_urls(self.settings.get('URLs')) or {}
-        collected_urls = dict()
-        collect_urls('', urls, collected_urls)
-        config['urls'] = finalize_urls(collected_urls)
-        logger.debug('Configs loaded.')
-        if config['monitoring']:
-            logger.info('Run "panther monitor" in another session for Monitoring.')
-
-    def _check_configs(self):
-        from panther.logger import logger
-        """Read the config file and put it as dict in self.settings"""
-        try:
-            configs_path = self.base_dir / 'core/configs.py'
-            self.settings = run_path(str(configs_path))
-        except FileNotFoundError:
-            logger.critical('core/configs.py Not Found.')
-
-    def _get_secret_key(self) -> bytes | None:
-        if secret_key := self.settings.get('SECRET_KEY'):
-            return secret_key.encode()
-        return None
-
-    def _get_authentication_class(self) -> ModelMetaclass | None:
-        return self.settings.get('AUTHENTICATION') and import_class(self.settings['AUTHENTICATION'])
-
-    def _get_user_model(self) -> ModelMetaclass:
-        return import_class(self.settings.get('USER_MODEL', 'panther.db.models.User'))
-
-    def _get_jwt_config(self) -> JWTConfig:
-        """Only Collect JWT Config If Authentication Is JWTAuthentication"""
-        if getattr(config['authentication'], '__name__', None) == 'JWTAuthentication':
-            user_config = self.settings.get('JWTConfig')
-            return JWTConfig(**user_config) if user_config else JWTConfig(key=config['secret_key'].decode())
-
-    def _get_middlewares(self) -> list:
-        """Collect The Middlewares & Set db_engine If One Of Middlewares Was For DB"""
-        from panther.logger import logger
-        middlewares = list()
-
-        for path, data in self.settings.get('MIDDLEWARES', []):
-            if path.find('panther.middlewares.db.Middleware') != -1:
-                config['db_engine'] = data['url'].split(':')[0]
-
-            Middleware = import_class(path)  # NOQA: Py Pep8 Naming
-            if not issubclass(Middleware, BaseMiddleware):
-                logger.critical(f'{Middleware} is not a sub class of BaseMiddleware.')
-                continue
-
-            middlewares.append(Middleware(**data))  # NOQA: Py Argument List
-        return middlewares
```

### Comparing `panther-1.7.3/panther/middlewares/monitoring.py` & `panther-1.7.4/panther/middlewares/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/middlewares/redis.py` & `panther-1.7.4/panther/middlewares/redis.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/request.py` & `panther-1.7.4/panther/request.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/response.py` & `panther-1.7.4/panther/response.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/routings.py` & `panther-1.7.4/panther/routings.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 
 def merge(destination: MutableMapping, *sources) -> MutableMapping:
     """Credit to Travis Clarke --> https://github.com/clarketm/mergedeep"""
     return reduce(partial(deepmerge), sources, destination)
 
 
-def finalize_urls(urls: dict):
+def finalize_urls(urls: dict) -> dict:
     urls_list = list()
     for url, endpoint in urls.items():
         path = dict()
         for single_path in url.split('/')[:-1][::-1]:
             path = {single_path: path or endpoint}
         urls_list.append(path)
     return merge(*urls_list)
```

### Comparing `panther-1.7.3/panther/status.py` & `panther-1.7.4/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther/utils.py` & `panther-1.7.4/panther/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/panther.egg-info/PKG-INFO` & `panther-1.7.4/panther.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.3
+Version: 1.7.4
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE
 
 ## Panther 
-<b>Is A Fast &  Friendly, Web Framework For Building Async APIs With Python 3.11+</b> 
+<b>Is A Fast &  Friendly Web Framework For Building Async APIs With Python 3.11+</b> 
 
 <p align="center">
 <img src="https://github.com/AliRn76/panther/raw/master/docs/docs/images/logo.png" alt="logo" style="width: 200px">
 </p>
 
 >_Full Documentation_ -> [https://pantherpy.github.io](https://pantherpy.github.io)
 >
```

### Comparing `panther-1.7.3/panther.egg-info/SOURCES.txt` & `panther-1.7.4/panther.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panther-1.7.3/setup.py` & `panther-1.7.4/setup.py`

 * *Files identical despite different names*

