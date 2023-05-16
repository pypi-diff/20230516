# Comparing `tmp/ho-protocols-0.2.6.tar.gz` & `tmp/ho-protocols-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ho-protocols-0.2.6.tar", last modified: Fri May 12 12:10:13 2023, max compression
+gzip compressed data, was "ho-protocols-0.2.7.tar", last modified: Tue May 16 07:55:44 2023, max compression
```

## Comparing `ho-protocols-0.2.6.tar` & `ho-protocols-0.2.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.226176 ho-protocols-0.2.6/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.2.6/LICENCE
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-12 12:10:13.226176 ho-protocols-0.2.6/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.2.6/README.md
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-05-12 12:10:13.226176 ho-protocols-0.2.6/setup.cfg
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1084 2023-04-25 09:43:50.000000 ho-protocols-0.2.6/setup.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.218176 ho-protocols-0.2.6/src/
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.222176 ho-protocols-0.2.6/src/ho_protocols/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.2.6/src/ho_protocols/__init__.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.222176 ho-protocols-0.2.6/src/ho_protocols/alert/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.2.6/src/ho_protocols/alert/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/alert/alert_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/alert/alert_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/alert/bees_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/alert/bees_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/alert/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/alert/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.222176 ho-protocols-0.2.6/src/ho_protocols/cmd/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.2.6/src/ho_protocols/cmd/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/cmd/cmd_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/cmd/cmd_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/common_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/common_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/data_in_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/data_in_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/example_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/example_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.226176 ho-protocols-0.2.6/src/ho_protocols/live/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.2.6/src/ho_protocols/live/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/actuators_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/actuators_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/live_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/live_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/models_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/models_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4245 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/sensors_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10173 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/sensors_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1483 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1972 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/live/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.226176 ho-protocols-0.2.6/src/ho_protocols/map/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.2.6/src/ho_protocols/map/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4556 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/map/map_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10813 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/map/map_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.226176 ho-protocols-0.2.6/src/ho_protocols/query/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.2.6/src/ho_protocols/query/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     7411 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/query/query_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    19694 2023-05-12 12:10:00.000000 ho-protocols-0.2.6/src/ho_protocols/query/query_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.222176 ho-protocols-0.2.6/src/ho_protocols.egg-info/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-12 12:10:13.000000 ho-protocols-0.2.6/src/ho_protocols.egg-info/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-05-12 12:10:13.000000 ho-protocols-0.2.6/src/ho_protocols.egg-info/SOURCES.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-05-12 12:10:13.000000 ho-protocols-0.2.6/src/ho_protocols.egg-info/dependency_links.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-05-12 12:10:13.000000 ho-protocols-0.2.6/src/ho_protocols.egg-info/requires.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-05-12 12:10:13.000000 ho-protocols-0.2.6/src/ho_protocols.egg-info/top_level.txt
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-12 12:10:13.226176 ho-protocols-0.2.6/test/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.2.6/test/test.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.170607 ho-protocols-0.2.7/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.2.7/LICENCE
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-16 07:55:44.170607 ho-protocols-0.2.7/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.2.7/README.md
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-05-16 07:55:44.170607 ho-protocols-0.2.7/setup.cfg
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1084 2023-04-25 09:43:50.000000 ho-protocols-0.2.7/setup.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.158608 ho-protocols-0.2.7/src/
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.162608 ho-protocols-0.2.7/src/ho_protocols/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.2.7/src/ho_protocols/__init__.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.166607 ho-protocols-0.2.7/src/ho_protocols/alert/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.2.7/src/ho_protocols/alert/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/alert/alert_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/alert/alert_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/alert/bees_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/alert/bees_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/alert/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/alert/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.166607 ho-protocols-0.2.7/src/ho_protocols/cmd/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.2.7/src/ho_protocols/cmd/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/cmd/cmd_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/cmd/cmd_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/common_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/common_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/data_in_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/data_in_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/example_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/example_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.170607 ho-protocols-0.2.7/src/ho_protocols/live/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.2.7/src/ho_protocols/live/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3608 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/actuators_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     8235 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/actuators_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/live_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/live_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/models_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/models_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4245 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/sensors_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10173 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/sensors_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2513 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5322 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/live/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.170607 ho-protocols-0.2.7/src/ho_protocols/map/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.2.7/src/ho_protocols/map/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4556 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/map/map_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10813 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/map/map_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.170607 ho-protocols-0.2.7/src/ho_protocols/query/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.2.7/src/ho_protocols/query/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     7411 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/query/query_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    19694 2023-05-16 07:55:38.000000 ho-protocols-0.2.7/src/ho_protocols/query/query_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.166607 ho-protocols-0.2.7/src/ho_protocols.egg-info/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-16 07:55:44.000000 ho-protocols-0.2.7/src/ho_protocols.egg-info/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-05-16 07:55:44.000000 ho-protocols-0.2.7/src/ho_protocols.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-05-16 07:55:44.000000 ho-protocols-0.2.7/src/ho_protocols.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-05-16 07:55:44.000000 ho-protocols-0.2.7/src/ho_protocols.egg-info/requires.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-05-16 07:55:44.000000 ho-protocols-0.2.7/src/ho_protocols.egg-info/top_level.txt
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-16 07:55:44.170607 ho-protocols-0.2.7/test/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.2.7/test/test.py
```

### Comparing `ho-protocols-0.2.6/LICENCE` & `ho-protocols-0.2.7/LICENCE`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/PKG-INFO` & `ho-protocols-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.2.6
+Version: 0.2.7
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.2.6/README.md` & `ho-protocols-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/setup.py` & `ho-protocols-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/alert/alert_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/alert/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/alert/alert_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/alert/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/alert/bees_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/alert/bees_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/alert/bees_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/alert/bees_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/alert/system_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/alert/system_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/alert/system_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/alert/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/cmd/cmd_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/cmd/cmd_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/cmd/cmd_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/cmd/cmd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/common_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/common_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/data_in_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/data_in_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/data_in_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/data_in_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/example_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/example_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/example_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/live/actuators_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/live/actuators_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,33 +9,35 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!ho_protocols/live/actuators.proto\x12\x11ho.live.actuators\"\xe3\x01\n\x10\x41\x63tuatorLiveItem\x12\x31\n\tbroodnest\x18\x01 \x01(\x0b\x32\x1c.ho.live.actuators.BroodnestH\x00\x12\'\n\x04gate\x18\x02 \x01(\x0b\x32\x17.ho.live.actuators.GateH\x00\x12\x33\n\x04\x65vac\x18\x03 \x01(\x0b\x32#.ho.live.actuators.EvacuationSystemH\x00\x12\x31\n\tharvester\x18\x04 \x01(\x0b\x32\x1c.ho.live.actuators.HarvesterH\x00\x42\x0b\n\tactuators\"5\n\tBroodnest\x12\x13\n\x0btarget_temp\x18\x01 \x01(\x02\x12\x13\n\x0b\x61\x63tual_temp\x18\x02 \x01(\x02\"\x9c\x01\n\x04Gate\x12.\n\x06status\x18\x01 \x01(\x0e\x32\x1e.ho.live.actuators.Gate.Status\x12\x10\n\x08position\x18\x02 \x01(\x02\"R\n\x06Status\x12\x0b\n\x07Unknown\x10\x00\x12\x0b\n\x07Opening\x10\x01\x12\x08\n\x04Open\x10\x02\x12\x0b\n\x07\x43losing\x10\x03\x12\n\n\x06\x43losed\x10\x04\x12\x0b\n\x07\x46\x61ilure\x10\x63\"\x9a\x01\n\x10\x45vacuationSystem\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.ho.live.actuators.EvacuationSystem.Status\x12\x0c\n\x04rate\x18\x02 \x01(\x02\"<\n\x06Status\x12\x0b\n\x07Unknown\x10\x00\x12\x0b\n\x07Stopped\x10\x01\x12\x0b\n\x07Working\x10\x02\x12\x0b\n\x07\x46\x61ilure\x10\x63\"\xa6\x01\n\tHarvester\x12\x33\n\x06status\x18\x01 \x01(\x0e\x32#.ho.live.actuators.Harvester.Status\x12\x10\n\x08position\x18\x02 \x01(\x02\"R\n\x06Status\x12\x0b\n\x07Unknown\x10\x00\x12\x0b\n\x07Opening\x10\x01\x12\x08\n\x04Open\x10\x02\x12\x0b\n\x07\x43losing\x10\x03\x12\n\n\x06\x43losed\x10\x04\x12\x0b\n\x07\x46\x61ilure\x10\x63\x42\x02H\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!ho_protocols/live/actuators.proto\x12\x11ho.live.actuators\"\xea\x01\n\x10\x41\x63tuatorLiveItem\x12\x38\n\rbroodnest_htr\x18\x01 \x01(\x0b\x32\x1f.ho.live.actuators.BroodnestHtrH\x00\x12\'\n\x04gate\x18\x02 \x01(\x0b\x32\x17.ho.live.actuators.GateH\x00\x12\x33\n\x04\x65vac\x18\x03 \x01(\x0b\x32#.ho.live.actuators.EvacuationSystemH\x00\x12\x31\n\tharvester\x18\x04 \x01(\x0b\x32\x1c.ho.live.actuators.HarvesterH\x00\x42\x0b\n\tactuators\"\xc1\x01\n\x0c\x42roodnestHtr\x12;\n\tactuators\x18\x01 \x03(\x0b\x32(.ho.live.actuators.BroodnestHtr.Actuator\x1at\n\x08\x41\x63tuator\x12\x19\n\x11\x61\x63tuator_instance\x18\x01 \x01(\t\x12\x0b\n\x03obj\x18\x02 \x01(\x02\x12\x0e\n\x06status\x18\x03 \x01(\x05\x12\x10\n\x08\x61vg_temp\x18\x04 \x01(\x02\x12\x0b\n\x03pwm\x18\x05 \x01(\x02\x12\x11\n\tis_active\x18\x06 \x01(\x05\"\x9c\x01\n\x04Gate\x12.\n\x06status\x18\x01 \x01(\x0e\x32\x1e.ho.live.actuators.Gate.Status\x12\x10\n\x08position\x18\x02 \x01(\x02\"R\n\x06Status\x12\x0b\n\x07Unknown\x10\x00\x12\x0b\n\x07Opening\x10\x01\x12\x08\n\x04Open\x10\x02\x12\x0b\n\x07\x43losing\x10\x03\x12\n\n\x06\x43losed\x10\x04\x12\x0b\n\x07\x46\x61ilure\x10\x63\"\x9a\x01\n\x10\x45vacuationSystem\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.ho.live.actuators.EvacuationSystem.Status\x12\x0c\n\x04rate\x18\x02 \x01(\x02\"<\n\x06Status\x12\x0b\n\x07Unknown\x10\x00\x12\x0b\n\x07Stopped\x10\x01\x12\x0b\n\x07Working\x10\x02\x12\x0b\n\x07\x46\x61ilure\x10\x63\"\xa6\x01\n\tHarvester\x12\x33\n\x06status\x18\x01 \x01(\x0e\x32#.ho.live.actuators.Harvester.Status\x12\x10\n\x08position\x18\x02 \x01(\x02\"R\n\x06Status\x12\x0b\n\x07Unknown\x10\x00\x12\x0b\n\x07Opening\x10\x01\x12\x08\n\x04Open\x10\x02\x12\x0b\n\x07\x43losing\x10\x03\x12\n\n\x06\x43losed\x10\x04\x12\x0b\n\x07\x46\x61ilure\x10\x63\x42\x02H\x03\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ho_protocols.live.actuators_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'H\003'
   _globals['_ACTUATORLIVEITEM']._serialized_start=57
-  _globals['_ACTUATORLIVEITEM']._serialized_end=284
-  _globals['_BROODNEST']._serialized_start=286
-  _globals['_BROODNEST']._serialized_end=339
-  _globals['_GATE']._serialized_start=342
-  _globals['_GATE']._serialized_end=498
-  _globals['_GATE_STATUS']._serialized_start=416
-  _globals['_GATE_STATUS']._serialized_end=498
-  _globals['_EVACUATIONSYSTEM']._serialized_start=501
-  _globals['_EVACUATIONSYSTEM']._serialized_end=655
-  _globals['_EVACUATIONSYSTEM_STATUS']._serialized_start=595
-  _globals['_EVACUATIONSYSTEM_STATUS']._serialized_end=655
-  _globals['_HARVESTER']._serialized_start=658
-  _globals['_HARVESTER']._serialized_end=824
-  _globals['_HARVESTER_STATUS']._serialized_start=416
-  _globals['_HARVESTER_STATUS']._serialized_end=498
+  _globals['_ACTUATORLIVEITEM']._serialized_end=291
+  _globals['_BROODNESTHTR']._serialized_start=294
+  _globals['_BROODNESTHTR']._serialized_end=487
+  _globals['_BROODNESTHTR_ACTUATOR']._serialized_start=371
+  _globals['_BROODNESTHTR_ACTUATOR']._serialized_end=487
+  _globals['_GATE']._serialized_start=490
+  _globals['_GATE']._serialized_end=646
+  _globals['_GATE_STATUS']._serialized_start=564
+  _globals['_GATE_STATUS']._serialized_end=646
+  _globals['_EVACUATIONSYSTEM']._serialized_start=649
+  _globals['_EVACUATIONSYSTEM']._serialized_end=803
+  _globals['_EVACUATIONSYSTEM_STATUS']._serialized_start=743
+  _globals['_EVACUATIONSYSTEM_STATUS']._serialized_end=803
+  _globals['_HARVESTER']._serialized_start=806
+  _globals['_HARVESTER']._serialized_end=972
+  _globals['_HARVESTER_STATUS']._serialized_start=564
+  _globals['_HARVESTER_STATUS']._serialized_end=646
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ho-protocols-0.2.6/src/ho_protocols/live/actuators_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/live/actuators_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
+import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
@@ -16,57 +18,83 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
 class ActuatorLiveItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    BROODNEST_FIELD_NUMBER: builtins.int
+    BROODNEST_HTR_FIELD_NUMBER: builtins.int
     GATE_FIELD_NUMBER: builtins.int
     EVAC_FIELD_NUMBER: builtins.int
     HARVESTER_FIELD_NUMBER: builtins.int
     @property
-    def broodnest(self) -> global___Broodnest: ...
+    def broodnest_htr(self) -> global___BroodnestHtr: ...
     @property
     def gate(self) -> global___Gate: ...
     @property
     def evac(self) -> global___EvacuationSystem: ...
     @property
     def harvester(self) -> global___Harvester: ...
     def __init__(
         self,
         *,
-        broodnest: global___Broodnest | None = ...,
+        broodnest_htr: global___BroodnestHtr | None = ...,
         gate: global___Gate | None = ...,
         evac: global___EvacuationSystem | None = ...,
         harvester: global___Harvester | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["actuators", b"actuators", "broodnest", b"broodnest", "evac", b"evac", "gate", b"gate", "harvester", b"harvester"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["actuators", b"actuators", "broodnest", b"broodnest", "evac", b"evac", "gate", b"gate", "harvester", b"harvester"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["actuators", b"actuators"]) -> typing_extensions.Literal["broodnest", "gate", "evac", "harvester"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["actuators", b"actuators", "broodnest_htr", b"broodnest_htr", "evac", b"evac", "gate", b"gate", "harvester", b"harvester"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["actuators", b"actuators", "broodnest_htr", b"broodnest_htr", "evac", b"evac", "gate", b"gate", "harvester", b"harvester"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["actuators", b"actuators"]) -> typing_extensions.Literal["broodnest_htr", "gate", "evac", "harvester"] | None: ...
 
 global___ActuatorLiveItem = ActuatorLiveItem
 
 @typing_extensions.final
-class Broodnest(google.protobuf.message.Message):
+class BroodnestHtr(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TARGET_TEMP_FIELD_NUMBER: builtins.int
-    ACTUAL_TEMP_FIELD_NUMBER: builtins.int
-    target_temp: builtins.float
-    actual_temp: builtins.float
+    @typing_extensions.final
+    class Actuator(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        ACTUATOR_INSTANCE_FIELD_NUMBER: builtins.int
+        OBJ_FIELD_NUMBER: builtins.int
+        STATUS_FIELD_NUMBER: builtins.int
+        AVG_TEMP_FIELD_NUMBER: builtins.int
+        PWM_FIELD_NUMBER: builtins.int
+        IS_ACTIVE_FIELD_NUMBER: builtins.int
+        actuator_instance: builtins.str
+        obj: builtins.float
+        status: builtins.int
+        avg_temp: builtins.float
+        pwm: builtins.float
+        is_active: builtins.int
+        def __init__(
+            self,
+            *,
+            actuator_instance: builtins.str = ...,
+            obj: builtins.float = ...,
+            status: builtins.int = ...,
+            avg_temp: builtins.float = ...,
+            pwm: builtins.float = ...,
+            is_active: builtins.int = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["actuator_instance", b"actuator_instance", "avg_temp", b"avg_temp", "is_active", b"is_active", "obj", b"obj", "pwm", b"pwm", "status", b"status"]) -> None: ...
+
+    ACTUATORS_FIELD_NUMBER: builtins.int
+    @property
+    def actuators(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BroodnestHtr.Actuator]: ...
     def __init__(
         self,
         *,
-        target_temp: builtins.float = ...,
-        actual_temp: builtins.float = ...,
+        actuators: collections.abc.Iterable[global___BroodnestHtr.Actuator] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["actual_temp", b"actual_temp", "target_temp", b"target_temp"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["actuators", b"actuators"]) -> None: ...
 
-global___Broodnest = Broodnest
+global___BroodnestHtr = BroodnestHtr
 
 @typing_extensions.final
 class Gate(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Status:
         ValueType = typing.NewType("ValueType", builtins.int)
```

### Comparing `ho-protocols-0.2.6/src/ho_protocols/live/live_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/live/live_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/live/live_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/live/live_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/live/models_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/live/models_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/live/models_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/live/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/live/sensors_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/live/sensors_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/live/sensors_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/live/sensors_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/live/system_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/live/system_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,27 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eho_protocols/live/system.proto\x12\x0eho.live.system\"\xc6\x01\n\x0eSystemLiveItem\x12\x12\n\ndisk_total\x18\x01 \x01(\x03\x12\x11\n\tdisk_used\x18\x02 \x01(\x03\x12\x11\n\tdisk_free\x18\x03 \x01(\x03\x12\x0f\n\x07load_1m\x18\x04 \x01(\x02\x12\x0f\n\x07load_5m\x18\x05 \x01(\x02\x12\x10\n\x08load_15m\x18\x06 \x01(\x02\x12\x11\n\tmem_total\x18\x07 \x01(\x03\x12\x10\n\x08mem_used\x18\x08 \x01(\x03\x12\x11\n\tmem_avail\x18\t \x01(\x03\x12\x0e\n\x06uptime\x18\n \x01(\x02\x42\x02H\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eho_protocols/live/system.proto\x12\x0eho.live.system\"\xaa\x01\n\x0eSystemLiveItem\x12/\n\ncore_stats\x18\x01 \x01(\x0b\x32\x19.ho.live.system.CoreStatsH\x00\x12+\n\x08\x63ore_pwr\x18\x02 \x01(\x0b\x32\x17.ho.live.system.CorePwrH\x00\x12\x32\n\x0c\x63ore_ip_addr\x18\x03 \x01(\x0b\x32\x1a.ho.live.system.CoreIPAddrH\x00\x42\x06\n\x04type\"\xc1\x01\n\tCoreStats\x12\x12\n\ndisk_total\x18\x01 \x01(\x03\x12\x11\n\tdisk_used\x18\x02 \x01(\x03\x12\x11\n\tdisk_free\x18\x03 \x01(\x03\x12\x0f\n\x07load_1m\x18\x04 \x01(\x02\x12\x0f\n\x07load_5m\x18\x05 \x01(\x02\x12\x10\n\x08load_15m\x18\x06 \x01(\x02\x12\x11\n\tmem_total\x18\x07 \x01(\x03\x12\x10\n\x08mem_used\x18\x08 \x01(\x03\x12\x11\n\tmem_avail\x18\t \x01(\x03\x12\x0e\n\x06uptime\x18\n \x01(\x02\"X\n\x07\x43orePwr\x12\t\n\x01v\x18\x01 \x01(\x02\x12\x0f\n\x07v_shunt\x18\x02 \x01(\x02\x12\r\n\x05power\x18\x03 \x01(\x02\x12\x0f\n\x07\x63urrent\x18\x04 \x01(\x02\x12\x11\n\tcurr_avg3\x18\x05 \x01(\x02\"c\n\nCoreIPAddr\x12.\n\x05items\x18\x01 \x03(\x0b\x32\x1f.ho.live.system.CoreIPAddr.Item\x1a%\n\x04Item\x12\x11\n\tinterface\x18\x01 \x01(\t\x12\n\n\x02ip\x18\x02 \x01(\tB\x02H\x03\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ho_protocols.live.system_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'H\003'
   _globals['_SYSTEMLIVEITEM']._serialized_start=51
-  _globals['_SYSTEMLIVEITEM']._serialized_end=249
+  _globals['_SYSTEMLIVEITEM']._serialized_end=221
+  _globals['_CORESTATS']._serialized_start=224
+  _globals['_CORESTATS']._serialized_end=417
+  _globals['_COREPWR']._serialized_start=419
+  _globals['_COREPWR']._serialized_end=507
+  _globals['_COREIPADDR']._serialized_start=509
+  _globals['_COREIPADDR']._serialized_end=608
+  _globals['_COREIPADDR_ITEM']._serialized_start=571
+  _globals['_COREIPADDR_ITEM']._serialized_end=608
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ho-protocols-0.2.6/src/ho_protocols/map/map_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/map/map_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/map/map_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/map/map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/query/query_pb2.py` & `ho-protocols-0.2.7/src/ho_protocols/query/query_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols/query/query_pb2.pyi` & `ho-protocols-0.2.7/src/ho_protocols/query/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/src/ho_protocols.egg-info/PKG-INFO` & `ho-protocols-0.2.7/src/ho_protocols.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.2.6
+Version: 0.2.7
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.2.6/src/ho_protocols.egg-info/SOURCES.txt` & `ho-protocols-0.2.7/src/ho_protocols.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.6/test/test.py` & `ho-protocols-0.2.7/test/test.py`

 * *Files identical despite different names*

