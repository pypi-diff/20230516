# Comparing `tmp/navabilitysdk-0.5.1.tar.gz` & `tmp/navabilitysdk-0.6.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navabilitysdk-0.5.1.tar", last modified: Fri Feb 24 01:17:49 2023, max compression
+gzip compressed data, was "navabilitysdk-0.6.0.post1.tar", last modified: Tue May 16 04:38:05 2023, max compression
```

## Comparing `navabilitysdk-0.5.1.tar` & `navabilitysdk-0.6.0.post1.tar`

### file list

```diff
@@ -1,50 +1,73 @@
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/
--rw-rw-r--   0 dehann    (1000) dehann    (1000)    11357 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/LICENSE
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      512 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/PKG-INFO
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     1130 2023-02-14 05:08:08.000000 navabilitysdk-0.5.1/README.md
--rw-rw-r--   0 dehann    (1000) dehann    (1000)       79 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/setup.cfg
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     1346 2023-02-23 07:42:57.000000 navabilitysdk-0.5.1/setup.py
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/
--rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/__init__.py
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/common/
--rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/common/__init__.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     3947 2023-02-21 02:44:09.000000 navabilitysdk-0.5.1/src/navability/common/mutations.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     9683 2023-02-20 22:14:11.000000 navabilitysdk-0.5.1/src/navability/common/queries.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      189 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/common/timestamps.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)       27 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/common/versions.py
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/entities/
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     1010 2023-02-24 00:34:43.000000 navabilitysdk-0.5.1/src/navability/entities/__init__.py
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/entities/blob/
--rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2023-02-20 15:50:38.000000 navabilitysdk-0.5.1/src/navability/entities/blob/__init__.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     2022 2023-02-20 22:14:11.000000 navabilitysdk-0.5.1/src/navability/entities/blob/blob.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      803 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/client.py
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/entities/factor/
--rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/factor/__init__.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     3600 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/factor/distributions.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     6457 2023-02-21 05:26:14.000000 navabilitysdk-0.5.1/src/navability/entities/factor/factor.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     8994 2023-02-23 07:42:57.000000 navabilitysdk-0.5.1/src/navability/entities/factor/inferencetypes.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     2792 2023-02-20 13:35:18.000000 navabilitysdk-0.5.1/src/navability/entities/navabilityclient.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      109 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/querydetail.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      967 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/scope.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      764 2022-07-07 20:02:22.000000 navabilitysdk-0.5.1/src/navability/entities/solve.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     1643 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/statusmessage.py
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.768212 navabilitysdk-0.5.1/src/navability/entities/variable/
--rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/variable/__init__.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     2046 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/entities/variable/ppe.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     7975 2023-02-13 22:28:36.000000 navabilitysdk-0.5.1/src/navability/entities/variable/variable.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     3144 2022-07-14 05:39:17.000000 navabilitysdk-0.5.1/src/navability/entities/variable/variablenodedata.py
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/src/navability/services/
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      152 2023-02-20 15:50:38.000000 navabilitysdk-0.5.1/src/navability/services/__init__.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     8754 2023-02-21 02:44:09.000000 navabilitysdk-0.5.1/src/navability/services/blob.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     5557 2022-07-07 20:02:22.000000 navabilitysdk-0.5.1/src/navability/services/factor.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      717 2022-07-07 20:02:22.000000 navabilitysdk-0.5.1/src/navability/services/solve.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     1664 2022-04-01 00:01:58.000000 navabilitysdk-0.5.1/src/navability/services/status.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     2910 2023-02-22 23:01:10.000000 navabilitysdk-0.5.1/src/navability/services/utils.py
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     8104 2023-02-20 15:50:38.000000 navabilitysdk-0.5.1/src/navability/services/variable.py
-drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-02-24 01:17:49.772213 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      512 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/PKG-INFO
--rw-rw-r--   0 dehann    (1000) dehann    (1000)     1379 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/SOURCES.txt
--rw-rw-r--   0 dehann    (1000) dehann    (1000)        1 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/dependency_links.txt
--rw-rw-r--   0 dehann    (1000) dehann    (1000)      143 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/requires.txt
--rw-rw-r--   0 dehann    (1000) dehann    (1000)       11 2023-02-24 01:17:49.000000 navabilitysdk-0.5.1/src/navabilitysdk.egg-info/top_level.txt
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.962717 navabilitysdk-0.6.0.post1/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)    11357 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/LICENSE
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)       31 2023-05-16 04:37:53.000000 navabilitysdk-0.6.0.post1/MANIFEST.in
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      520 2023-05-16 04:38:05.962717 navabilitysdk-0.6.0.post1/PKG-INFO
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1353 2023-05-11 06:42:05.000000 navabilitysdk-0.6.0.post1/README.md
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)       79 2023-05-16 04:38:05.962717 navabilitysdk-0.6.0.post1/setup.cfg
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     3241 2023-05-16 04:37:53.000000 navabilitysdk-0.6.0.post1/setup.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.958717 navabilitysdk-0.6.0.post1/src/
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.958717 navabilitysdk-0.6.0.post1/src/navability/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/__init__.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.958717 navabilitysdk-0.6.0.post1/src/navability/common/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/common/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      189 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/common/timestamps.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)       27 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/common/versions.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.958717 navabilitysdk-0.6.0.post1/src/navability/entities/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1056 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/__init__.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.958717 navabilitysdk-0.6.0.post1/src/navability/entities/blob/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/blob/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     5794 2023-05-15 08:23:44.000000 navabilitysdk-0.6.0.post1/src/navability/entities/blob/blobentry.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      839 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/client.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1693 2023-05-14 08:23:40.000000 navabilitysdk-0.6.0.post1/src/navability/entities/dfgclient.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.958717 navabilitysdk-0.6.0.post1/src/navability/entities/factor/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/factor/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     3600 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/factor/distributions.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     7477 2023-05-15 19:52:01.000000 navabilitysdk-0.6.0.post1/src/navability/entities/factor/factor.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     8994 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/factor/inferencetypes.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.958717 navabilitysdk-0.6.0.post1/src/navability/entities/map/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/map/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      867 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/map/affordance.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      704 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/map/annotation.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2046 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/map/map.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      713 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/map/visualizationblob.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1300 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/map/workflow.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     3013 2023-05-15 08:23:44.000000 navabilitysdk-0.6.0.post1/src/navability/entities/navabilityclient.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      109 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/querydetail.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2042 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/robot.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2585 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/session.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      764 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/solve.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2457 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/user.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.958717 navabilitysdk-0.6.0.post1/src/navability/entities/variable/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/variable/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2391 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/variable/ppe.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)    10258 2023-05-12 04:18:40.000000 navabilitysdk-0.6.0.post1/src/navability/entities/variable/variable.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     3222 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/entities/variable/variablenodedata.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.962717 navabilitysdk-0.6.0.post1/src/navability/services/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      280 2023-05-14 08:23:40.000000 navabilitysdk-0.6.0.post1/src/navability/services/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     5809 2023-05-15 08:23:44.000000 navabilitysdk-0.6.0.post1/src/navability/services/blobentry.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     4907 2023-05-11 07:26:30.000000 navabilitysdk-0.6.0.post1/src/navability/services/blobstore.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     8395 2023-05-15 19:52:01.000000 navabilitysdk-0.6.0.post1/src/navability/services/factor.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2065 2023-05-14 15:37:42.000000 navabilitysdk-0.6.0.post1/src/navability/services/graph.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     6362 2023-05-16 04:37:53.000000 navabilitysdk-0.6.0.post1/src/navability/services/loader.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1976 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/services/map.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1300 2023-05-09 17:29:42.000000 navabilitysdk-0.6.0.post1/src/navability/services/user.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)    12912 2023-05-12 04:18:40.000000 navabilitysdk-0.6.0.post1/src/navability/services/variable.py
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.962717 navabilitysdk-0.6.0.post1/src/navabilitysdk.egg-info/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      520 2023-05-16 04:38:05.000000 navabilitysdk-0.6.0.post1/src/navabilitysdk.egg-info/PKG-INFO
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2075 2023-05-16 04:38:05.000000 navabilitysdk-0.6.0.post1/src/navabilitysdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        1 2023-05-16 04:38:05.000000 navabilitysdk-0.6.0.post1/src/navabilitysdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      173 2023-05-16 04:38:05.000000 navabilitysdk-0.6.0.post1/src/navabilitysdk.egg-info/requires.txt
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)       24 2023-05-16 04:38:05.000000 navabilitysdk-0.6.0.post1/src/navabilitysdk.egg-info/top_level.txt
+drwxrwxr-x   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:38:05.962717 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)        0 2023-05-16 04:26:58.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/__init__.py
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     3625 2023-05-12 05:19:37.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/blobentries.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      955 2023-05-09 17:31:27.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/blobstores.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2240 2023-05-12 05:19:37.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/factors.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1332 2023-05-09 17:31:27.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/maps.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2703 2023-05-09 17:31:27.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/ppes.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      880 2023-05-11 03:35:20.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/robots.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     1123 2023-05-09 17:31:27.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/session.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     2993 2023-05-09 17:31:27.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/solverdata.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      780 2023-05-11 05:47:57.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/users.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)     5023 2023-05-14 08:23:50.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/variables.toml
+-rw-rw-r--   0 dehann    (1000) dehann    (1000)      657 2023-05-09 17:31:27.000000 navabilitysdk-0.6.0.post1/src/sdkCommonGQL/workflows.toml
```

### Comparing `navabilitysdk-0.5.1/LICENSE` & `navabilitysdk-0.6.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.1/PKG-INFO` & `navabilitysdk-0.6.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: navabilitysdk
-Version: 0.5.1
+Version: 0.6.0.post1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: NavAbility
 Author-email: info@navability.io
 License: Apache-2.0
-Download-URL: https://github.com/NavAbility/NavAbilitySDK.py/archive/refs/tags/v0.5.1.tar.gz
+Download-URL: https://github.com/NavAbility/NavAbilitySDK.py/archive/refs/tags/v0.6.0-1.tar.gz
 Description: NavAbility SDK: Access NavAbility Cloud factor graph features from Python.
         Note that this SDK and the related API are in beta. Please let us know if you have any issues at info@navability.io.
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `navabilitysdk-0.5.1/src/navability/entities/__init__.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,19 @@
     PriorPose3,
 )
 from .navabilityclient import (
     NavAbilityClient,
     NavAbilityHttpsClient,
     NavAbilityWebsocketClient,
 )
+
+from .dfgclient import DFGClient
+
 from .querydetail import QueryDetail
-from .scope import Scope
-from .solve import SolveOptions
-from .statusmessage import MutationUpdate, StatusMessage
+# from .scope import Scope
+# from .solve import SolveOptions
+# from .statusmessage import MutationUpdate, StatusMessage
 from .variable.ppe import Ppe
 from .variable.variable import Variable, VariableSkeleton, VariableSummary, VariableType
 from .variable.variablenodedata import VariableNodeData
 
-from .blob.blob import BlobEntry
+from .blob.blobentry import BlobEntry
```

### Comparing `navabilitysdk-0.5.1/src/navability/entities/client.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from dataclasses import dataclass
 
 from marshmallow import Schema, fields, post_load
 
 
 @dataclass()
 class Client:
-    userId: str
-    robotId: str
-    sessionId: str
+    userLabel: str
+    robotLabel: str
+    sessionLabel: str
 
     def __repr__(self):
-        return f"<Client(userId={self.userId}, robotId={self.robotId}, sessionId={self.sessionId})>"  # noqa: E501, B950
+        return f"<Client(userLabel={self.userLabel}, robotId={self.robotLabel}, sessionId={self.sessionLabel})>"  # noqa: E501, BLabeLabel
 
     def dump(self):
         return ClientSchema().dump(self)
 
     def dumps(self):
         return ClientSchema().dumps(self)
 
     @staticmethod
     def load(data):
         return ClientSchema().load(data)
 
 
 class ClientSchema(Schema):
-    userId = fields.String(required=True)
-    robotId = fields.String(required=True)
-    sessionId = fields.String(required=True)
+    userLabel = fields.String(required=True)
+    robotLabel = fields.String(required=True)
+    sessionLabel = fields.String(required=True)
 
     class Meta:
         ordered = True
 
     @post_load
     def marshal(self, data, **kwargs):
         return Client(**data)
```

### Comparing `navabilitysdk-0.5.1/src/navability/entities/factor/distributions.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/factor/distributions.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.1/src/navability/entities/factor/factor.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/factor/factor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Dict, List
+from uuid import UUID
 import json
 import base64
 
-from marshmallow import EXCLUDE, Schema, fields, post_load
+from marshmallow import EXCLUDE, Schema, fields, post_load, pre_load
 
 from navability.common.timestamps import TS_FORMAT
 from navability.common.versions import payload_version
 
 
 @dataclass()
 class FactorSkeleton:
+    id: UUID
     label: str
     variableOrderSymbols: List[str]
     tags: List[str]
 
     def __repr__(self):
         return (
             f"<FactorSkeleton(label={self.label},"
-            f"variableOrderSymbols={self.variableOrderSymbols},tags={self.tags})>"
+            f"variableOrderSymbols={self._variableOrderSymbols},tags={self.tags})>"
         )
 
     def dump(self):
         return FactorSkeletonSchema().dump(self)
 
     def dumps(self):
         return FactorSkeletonSchema().dumps(self)
 
     @staticmethod
     def load(data):
         return FactorSkeletonSchema().load(data)
 
 
 class FactorSkeletonSchema(Schema):
+    id = fields.UUID(required=True)
     label = fields.Str(required=True)
     variableOrderSymbols = fields.List(
         fields.Str, data_key="_variableOrderSymbols", required=True
     )
     tags = fields.List(fields.Str(), required=True)
 
     class Meta:
@@ -46,38 +49,40 @@
     @post_load
     def marshal(self, data, **kwargs):
         return FactorSkeleton(**data)
 
 
 @dataclass()
 class FactorSummary:
-    label = str
+    id: UUID
+    label: str
     variableOrderSymbols: List[str]
     tags: List[str] = field(default_factory=lambda: ["FACTOR"])
     timestamp: datetime = datetime.utcnow()
     _version: str = payload_version
 
     def __repr__(self):
         return (
             f"<FactorSkeleton(label={self.label},"
-            f"variableOrderSymbols={self.variableOrderSymbols},tags={self.tags})>"
+            f"variableOrderSymbols={self._variableOrderSymbols},tags={self.tags})>"
         )
 
     def dump(self):
         return FactorSummarySchema().dump(self)
 
     def dumps(self):
         return FactorSummarySchema().dumps(self)
 
     @staticmethod
     def load(data):
         return FactorSummarySchema().load(data)
 
 
 class FactorSummarySchema(Schema):
+    id = fields.UUID(required=True)
     label = fields.Str(required=True)
     variableOrderSymbols = fields.List(
         fields.Str, data_key="_variableOrderSymbols", required=True
     )
     tags = fields.List(fields.Str(), required=True)
     timestamp = fields.Method("get_timestamp", "set_timestamp", required=True)
     _version = fields.Str(required=True)
@@ -151,27 +156,29 @@
         return FactorData(**data)
 
 
 @dataclass()
 class Factor:
     label: str
     fnctype: str
-    variableOrderSymbols: List[str]
-    data: FactorData
+    _variableOrderSymbols: List[str]
+    data: str
+    metadata: str = "e30="
     tags: List[str] = field(default_factory=lambda: ["FACTOR"])
-    timestamp: str = datetime.utcnow()
-    nstime: int = 0
+    timestamp: datetime = datetime.utcnow()
+    nstime: str = "0"
     solvable: str = 1
     _version: str = payload_version
+    id: UUID = None
 
     def __repr__(self):
         return (
             f"<{self.__class__.__name__}"
             f"(label={self.label},"
-            f"variables={self.variableOrderSymbols})>"
+            f"variables={self._variableOrderSymbols})>"
         )
 
     def dump(self):
         return FactorSchema().dump(self)
 
     def dumps(self):
         return FactorSchema().dumps(self)
@@ -179,26 +186,41 @@
     @staticmethod
     def load(data):
         # import pdb; pdb.set_trace()
         return FactorSchema().load(data)
 
 
 class FactorSchema(Schema):
+    id = fields.UUID(required=True)
     label = fields.Str(required=True)
     _version = fields.Str(required=True)
-    variableOrderSymbols = fields.List(
+    _variableOrderSymbols = fields.List(
         fields.Str, data_key="_variableOrderSymbols", required=True
     )
     data = fields.Method("get_data", "set_data", required=True)
     tags = fields.List(fields.Str(), required=True)
     timestamp = fields.Method("get_timestamp", "set_timestamp", required=True)
     nstime = fields.Str(default="0")
     fnctype = fields.Str(required=True)
+    metadata = fields.Method("get_metadata", "set_metadata")
     solvable = fields.Int(required=True)
 
+    @pre_load
+    def b64_data_duel(self, factor, many=None, partial=None):
+        # print(type(factor['data']), isinstance(factor['data'], dict))
+        # yes, it's a duel here in SDK.py@v0.6.0
+        try:
+            json.loads(factor['data'])
+        except json.JSONDecodeError as err:
+            # discrepancy between DFG@v0.21.1 and SDK.jl@v0.6.0 in 
+            #  assume .data was b64 encoded by one of the other SDKs (expected in future)
+            factor['data'] = base64.b64decode(factor['data'])
+
+        return factor
+
     class Meta:
         ordered = True
         unknown = EXCLUDE  # Note: This is because of _version, remote and fix later.
 
     def get_timestamp(self, obj):
         # Return a robust timestamp
         ts = obj.timestamp.isoformat(timespec="milliseconds")
@@ -209,17 +231,24 @@
     def set_timestamp(self, obj):
         # Have to be defensive here because it could be simply serialized
         # or it can be GQL data with formatted
         tsraw = obj if type(obj) == str else obj["formatted"]
         return datetime.strptime(tsraw, TS_FORMAT)
 
     def get_data(self, obj):
-        return obj.data.dump()
+        return json.dumps(obj.data.dumps())
+
+    def set_data(self, obj):
+        return FactorDataSchema().load(json.loads(obj))
+
+    def get_metadata(self, obj):
+        return base64.b64encode(json.dumps(obj).encode())
 
-    def set_data(self, ob):
-        db64 = base64.b64decode(ob)
-        return FactorDataSchema().load(json.loads(db64))
-        
+    def set_metadata(self, obj):
+        if obj == '':
+            return {}
+        else:
+            return json.loads(base64.b64decode(obj))
 
     @post_load
     def marshal(self, data, **kwargs):
         return Factor(**data)
```

### Comparing `navabilitysdk-0.5.1/src/navability/entities/factor/inferencetypes.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/factor/inferencetypes.py`

 * *Files identical despite different names*

### Comparing `navabilitysdk-0.5.1/src/navability/entities/navabilityclient.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/navabilityclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,18 +53,20 @@
                 f"Calling mutation {options.mutation} with args: {options.variables}"
             )
             result = await client.execute(options.mutation, options.variables)
             return result
 
 
 class NavAbilityHttpsClient(NavAbilityClient):
-    """Connection object for queries and mutations to API server.
+    """Connection object for queries and mutations to API server.  Note, this is used but higher level objects such as DFGClient.
 
     Args:
-        NavAbilityClient (NavAbilityClient): the connection object
+        NavAbilityClient: the connection object to a server (cloud our deployed).
+        url: Network path to the API (cloud or deployed).
+        auth_token: Token for auth, likely provided by NavAbility App Connect page.
     """
     def __init__(self, url: str = "https://api.navability.io", auth_token: str = "") -> None:
         super().__init__()
         if len(auth_token) == 0:
             self.transport = AIOHTTPTransport(
                 url=url,
             )
```

### Comparing `navabilitysdk-0.5.1/src/navability/entities/scope.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/solve.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from dataclasses import dataclass, field
-from typing import List
+from dataclasses import dataclass
 
 from marshmallow import Schema, fields, post_load
 
 
 @dataclass()
-class Scope:
-    environmentIds: List[str] = field(default_factory=lambda: [])
-    userIds: List[str] = field(default_factory=lambda: [])
-    robotIds: List[str] = field(default_factory=lambda: [])
-    sessionIds: List[str] = field(default_factory=lambda: [])
+class SolveOptions:
+    key: str
+    useParametric: bool
+
+    def __repr__(self):
+        return f"<SolveOptions(key={self.key}, useParametric={self.useParametric})>"  # noqa: E501, B950
 
     def dump(self):
-        return ScopeSchema().dump(self)
+        return SolveOptionsSchema().dump(self)
 
     def dumps(self):
-        return ScopeSchema().dumps(self)
+        return SolveOptionsSchema().dumps(self)
 
     @staticmethod
-    def load(data: str):
-        return ScopeSchema().load(data)
+    def load(data):
+        return SolveOptionsSchema().load(data)
 
 
-class ScopeSchema(Schema):
-    environmentIds = fields.String(many=True, default=[])
-    userIds = fields.String(many=True, default=[])
-    robotIds = fields.String(many=True, default=[])
-    sessionIds = fields.String(many=True, default=[])
+class SolveOptionsSchema(Schema):
+    key = fields.String(required=True)
+    useParametric = fields.Bool(required=True)
 
     class Meta:
         ordered = True
 
     @post_load
     def marshal(self, data, **kwargs):
-        return Scope(**data)
+        return SolveOptions(**data)
```

### Comparing `navabilitysdk-0.5.1/src/navability/entities/variable/ppe.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/variable/ppe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from dataclasses import dataclass
 from datetime import datetime, timezone
-from typing import List
+from typing import List, Optional
+from uuid import UUID
 
 from marshmallow import Schema, fields, post_load
 
 from navability.common.timestamps import TS_FORMAT, TS_FORMAT_NO_TZ
 
-
+#TODO should we rename to MeanMaxPPE?
 @dataclass()
 class Ppe:
+    id: Optional[UUID]
     solveKey: str
     suggested: List[float]
     max: List[float]
     mean: List[float]
+    _type: str
+    _version: str
+    createdTimestamp: datetime
     lastUpdatedTimestamp: datetime
 
     def __repr__(self):
         return (
             f"<Ppe(solveKey={self.solveKey},suggested={self.suggested},"
             f"lastUpdatedTimestamp={self.lastUpdatedTimestamp})>"
         )
@@ -29,18 +34,24 @@
 
     @staticmethod
     def load(data):
         return PpeSchema().load(data)
 
 
 class PpeSchema(Schema):
+    id = fields.UUID()
     solveKey = fields.Str(required=True)
     suggested = fields.List(fields.Float(), required=True)
     max = fields.List(fields.Float(), required=True)
     mean = fields.List(fields.Float(), required=True)
+    _type = fields.Str()
+    _version = fields.Str(required=True)
+    createdTimestamp = fields.Method(
+        "get_timestamp", "set_timestamp", required=True
+    )
     lastUpdatedTimestamp = fields.Method(
         "get_timestamp", "set_timestamp", required=True
     )
 
     class Meta:
         ordered = True
```

### Comparing `navabilitysdk-0.5.1/src/navability/entities/variable/variable.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/variable/variable.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import base64
 import json
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
-from typing import Dict, List
+from typing import Dict, List, Optional
+from uuid import UUID
 
 from marshmallow import EXCLUDE, Schema, fields, post_load
 
 from navability.common.timestamps import TS_FORMAT
 from navability.common.versions import payload_version
 from navability.entities.variable.ppe import Ppe, PpeSchema
+from navability.entities.blob.blobentry import BlobEntry, BlobEntrySchema
 from navability.entities.variable.variablenodedata import (
     VariableNodeData,
     VariableNodeDataSchema,
 )
 
 
 class VariableType(Enum):
@@ -36,34 +39,38 @@
         return VariableNodeData(variableType, solveKey, 2)
     if variableType == "RoME.Pose2":
         return VariableNodeData(variableType, solveKey, 3)
     if variableType == "RoME.Pose3":
         return VariableNodeData(variableType, solveKey, 6)
     if variableType == "IncrementalInference.ContinuousScalar":
         return VariableNodeData(variableType, solveKey, 1)
+    if variableType == "Position{1}":
+        return VariableNodeData(variableType, solveKey, 1)
     raise Exception(f"Variable type '{variableType}' not supported.")
 
 
 @dataclass()
 class VariableSkeleton:
     label: str
     tags: List[str] = field(default_factory=lambda: ["VARIABLE"])
+    id: Optional[UUID] = None
 
     def dump(self):
         return VariableSkeletonSchema().dump(self)
 
     def dumps(self):
         return VariableSkeletonSchema().dumps(self)
 
     @staticmethod
     def load(data):
         return VariableSkeletonSchema().load(data)
 
 
 class VariableSkeletonSchema(Schema):
+    id = fields.UUID(required=True)
     label = fields.Str(required=True)
     tags = fields.List(fields.Str(), required=True)
 
     class Meta:
         ordered = True
 
     @post_load
@@ -72,18 +79,22 @@
 
 
 @dataclass()
 class VariableSummary:
     label: str
     variableType: str
     tags: List[str] = field(default_factory=lambda: ["VARIABLE"])
-    ppes: Dict[str, Ppe] = field(default_factory=lambda: {})
     timestamp: datetime = datetime.utcnow()
+    nstime: str = "0"
+    # ppes: Dict[str, Ppe] = field(default_factory=lambda: {})
+    ppes: List[Ppe] = field(default_factory=lambda: [])
+    # blobEntries: Dict[str, BlobEntry] = field(default_factory=lambda: {})
+    blobEntries: List[BlobEntry] = field(default_factory=lambda: [])
     _version: str = payload_version
-    _id: int = None
+    id: Optional[UUID] = None
 
     def __repr__(self):
         return (
             f"<VariableSummary(label={self.label},"
             f"variableType={self.variableType},tags={self.tags})>"
         )
 
@@ -95,62 +106,81 @@
 
     @staticmethod
     def load(data):
         return VariableSummarySchema().load(data)
 
 
 class VariableSummarySchema(Schema):
+    id = fields.UUID()
     label = fields.Str(required=True)
+    variableType = fields.Str(required=True)
     tags = fields.List(fields.Str())
-    ppes = fields.Nested(PpeSchema, many=True)
     timestamp = fields.Method("get_timestamp", "set_timestamp", required=True)
-    variableType = fields.Str(required=True)
+    nstime = fields.Str(default="0")
+    ppes = fields.Nested(PpeSchema, many=True)
+    # ppes = fields.Method("get_ppes", "set_ppes")
+    blobEntries = fields.Nested(BlobEntrySchema, many=True)
     _version = fields.Str(required=True)
-    _id = fields.Integer(data_key="_id", required=False)
 
     class Meta:
         ordered = True
 
     def get_timestamp(self, obj):
         # Return a robust timestamp
         ts = obj.timestamp.isoformat(timespec="milliseconds")
         if not obj.timestamp.tzinfo:
             ts += "+00"
         return ts
 
     def set_timestamp(self, obj):
-        return datetime.strptime(obj["formatted"], TS_FORMAT)
+        tsraw = obj if type(obj) == str else obj["formatted"]
+        return datetime.strptime(tsraw, TS_FORMAT)
 
     @post_load
     def marshal(self, data, **kwargs):
         return VariableSummary(**data)
 
 
 @dataclass()
 class Variable:
+    """A factor graph variable node as well as data carrying object that can serialized and distributed across computing nodes.
+
+    Parameters:
+        label: The variable label, such as "x1" or "pose_7"
+        variableType: For example "Pose2" or "Pose3"
+        tags: A string list of tags for annotating and later searching through nodes, e.g. ["POSE", "VARIABLE", "AUTO"]
+        timestamp: When the variable instance occurred.
+        nstime: duplicate ns scale time information which does not store full unix time, but rather only the nanosecond portion for higher resolution.
+        solvable: indicate whether the variable is ready to be incldued in a solve.
+        ppes: Parametric point estimate solutions which summarize the possibly non-Gaussian solution contained in `.solverData`.
+        blobEntries: A list of `BlobEntry`s which holds contextual information for (data) `Blob`s stored in a separate `BlobStore`.
+        solverData: In depth solver information used for numerical solutions of the factor graph, including non-Gaussian and multiple `solveKeys`.
+        metadata: To store opportunistic "small data" that migth be useful to keep.  Use BlobEntries and Blobs as main mechanism for storing heavy lift data.
+        _version: Serialization support of Variable objects benefit from knowing the library version used for this object.
+        id: Autogenerated uuid4 for use in a distributed system, do not self assign.
+    """
     label: str
     variableType: str
     tags: List[str] = field(default_factory=lambda: ["VARIABLE"])
-    ppes: Dict[str, Ppe] = field(default_factory=lambda: {})
     timestamp: datetime = datetime.utcnow()
-    nstime: int = 0
-    dataEntry: str = "{}"
-    dataEntryType: str = "{}"
-    solverData: Dict[str, VariableNodeData] = field(default_factory=lambda: {})
-    smallData: str = "{}"
+    nstime: str = "0"
     solvable: str = 1
+    ppes: Dict[str, Ppe] = field(default_factory=lambda: {})
+    blobEntries: Dict[str, BlobEntry] = field(default_factory=lambda: {})
+    solverData: Dict[str, VariableNodeData] = field(default_factory=lambda: {})
+    metadata: dict = field(default_factory=lambda: {})
     _version: str = payload_version
-    _id: int = None
+    id: Optional[UUID] = None
 
-    def __post_init__(self):
-        pass
-        if self.solverData == {}:
-            self.solverData["default"] = _getVariableNodeData(
-                self.variableType, "default"
-            )
+    # def __post_init__(self):
+    #     pass
+    #     if self.solverData == {}:
+    #         self.solverData["default"] = _getVariableNodeData(
+    #             self.variableType, "default"
+    #         )
 
     def __repr__(self):
         return (
             f"<Variable(label={self.label},variableType={self.variableType},"
             f"tags={self.tags})>"
         )
 
@@ -168,26 +198,26 @@
 
     @staticmethod
     def load(data):
         return VariableSchema().load(data)
 
 
 class VariableSchema(Schema):
+    id = fields.UUID()
     label = fields.Str(required=True)
+    variableType = fields.Str(required=True)
     tags = fields.List(fields.Str(), required=True)
-    ppes = fields.Method("get_ppes", "set_ppes")
     timestamp = fields.Method("get_timestamp", "set_timestamp", required=True)
-    variableType = fields.Str(required=True)
-    _version = fields.Str(required=True)
-    _id: fields.Integer(data_key="_id", required=False)
-    # dataEntry = fields.Str(required=True)
-    # dataEntryType = fields.Str(required=True)
-    solverData = fields.Method("get_solverdata", "set_solverdata")
-    smallData = fields.Str(required=True)
+    nstime = fields.Str(default="0")
     solvable = fields.Int(required=True)
+    ppes = fields.Method("get_ppes", "set_ppes")
+    blobEntries = fields.Nested(BlobEntrySchema, many=True)
+    solverData = fields.Method("get_solverdata", "set_solverdata")
+    metadata = fields.Method("get_metadata", "set_metadata")
+    _version = fields.Str(required=True)
 
     class Meta:
         ordered = True
         unknown = EXCLUDE  # Note: This is because of _id, remote and fix later.
 
     @post_load
     def marshal(self, data, **kwargs):
@@ -214,26 +244,30 @@
 
     def get_ppes(self, obj):
         return [ppe.dump() for ppe in obj.ppes.values()]
 
     def set_ppes(self, obj):
         return {ppe["solveKey"]: PpeSchema().load(ppe) for ppe in obj}
 
+    def get_metadata(self, obj):
+        return base64.b64encode(json.dumps(obj).encode())
+
+    def set_metadata(self, obj):
+        return json.loads(base64.b64decode(obj))
+
 
 class PackedVariableSchema(Schema):
     """
     A special schema for the addVariable call, which is used to
     form a packed variable struct.
     """
 
     label = fields.Str(required=True)
-    dataEntry = fields.Str(required=True)
     nstime = fields.Str(default="0")
     variableType = fields.Str(required=True)
-    dataEntryType = fields.Str(required=True)
     ppeDict = fields.Str(attribute="ppes", required=True)
     solverDataDict = fields.Method("get_solver_data_dict", required=True)
     smallData = fields.Str(required=True)
     solvable = fields.Int(required=True)
     tags = fields.List(fields.Str(), required=True)
     timestamp = fields.Method("get_timestamp", required=True)
     _version = fields.Str(required=True)
```

### Comparing `navabilitysdk-0.5.1/src/navability/entities/variable/variablenodedata.py` & `navabilitysdk-0.6.0.post1/src/navability/entities/variable/variablenodedata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from dataclasses import dataclass, field
-from typing import List
+from typing import List, Optional
+from uuid import UUID
 
 import numpy
 from marshmallow import EXCLUDE, Schema, fields, post_load
 
 from navability.common.versions import payload_version
 
 
 @dataclass()
 class VariableNodeData:
+    id: Optional[UUID]
     variableType: str
     solveKey: str
     dims: int
     vecval: List[float] = None
     dimval: int = 0
     vecbw: List[float] = None
     dimbw: int = 0
@@ -56,14 +58,15 @@
 
     @staticmethod
     def load(data):
         return VariableNodeDataSchema().load(data)
 
 
 class VariableNodeDataSchema(Schema):
+    id = fields.UUID()
     vecval = fields.List(fields.Float(), required=True)  # numpy.zeros(3*100) # 300
     dimval = fields.Integer(required=True)  # 3
     vecbw = fields.List(fields.Float(), required=True)  # numpy.zeros(3)
     dimbw = fields.Integer(required=True)  # 3
     BayesNetOutVertIDs = fields.List(fields.Integer(), required=True)  # []
     dimIDs = fields.List(fields.Integer(), required=True)  # [0,1,2]
     dims = fields.Integer(required=True)  # 3
```

### Comparing `navabilitysdk-0.5.1/src/navability/services/blob.py` & `navabilitysdk-0.6.0.post1/src/navability/services/factor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,335 +1,296 @@
 import logging
-import warnings
-import requests
 from typing import List
+from uuid import uuid4
 
 from gql import gql
 
-from navability.common.queries import (
-    GQL_LISTDATAENTRIES,
-)
-from navability.common.mutations import (
-    GQL_CREATEDOWNLOAD,
-    GQL_CREATEUPLOAD,
-    GQL_COMPLETEUPLOAD_SINGLE,
-    GQL_ADDBLOBENTRY,
-)
+import asyncio
+
+from navability.entities.dfgclient import DFGClient
+
 from navability.entities.client import Client
+
+from navability.services.loader import GQL_OPERATIONS
+from navability.entities.factor.factor import (
+    Factor,
+    FactorData,
+    FactorSchema,
+    FactorSkeleton,
+    FactorSkeletonSchema,
+    FactorSummarySchema,
+)
+from navability.entities.factor.inferencetypes import InferenceType
 from navability.entities.navabilityclient import (
     MutationOptions,
     NavAbilityClient,
     QueryOptions,
 )
-# from navability.entities.querydetail import QueryDetail
-from navability.entities.blob.blob import (
-    BlobEntry,
-    BlobEntrySchema,
-)
+from navability.entities.querydetail import QueryDetail
 
+import nest_asyncio
+nest_asyncio.apply()
+
+DETAIL_SCHEMA = {
+    QueryDetail.LABEL: None,
+    QueryDetail.SKELETON: FactorSkeletonSchema(),
+    QueryDetail.SUMMARY: FactorSummarySchema(),
+    QueryDetail.FULL: FactorSchema(),
+}
 
 logger = logging.getLogger(__name__)
 
-async def listBlobEntries(
-    client: NavAbilityClient,
-    context: Client,
-    variableLabel,
-):
-    """ List the blob entries associated with a particular variable.
 
-    Args:
-        client (NavAbilityClient): client connection to API server
-        context (Client): Unique context with (user, robot, session)
-        variableLabel (string): list data entries connected to which variable
+async def getFactorAsync(fgclient: DFGClient, label: str, debug=False):
 
-    Returns:
-        BlobEntry: coroutine containing a list of `BlobEntry`s
+    client = fgclient.client
+    context = fgclient.context
 
-    """
     params = {
-        "userId": context.userId,
-        "robotId": context.robotId,
-        "sessionId": context.sessionId,
-        "variableLabel": variableLabel,
+        "userLabel": context.userLabel,
+        "robotLabel": context.robotLabel,
+        "sessionLabel": context.sessionLabel,
+        "label": label,
+        # "fields_summary": detail in [QueryDetail.SUMMARY, QueryDetail.FULL],
+        # "fields_full": detail == QueryDetail.FULL,
     }
+
     logger.debug(f"Query params: {params}")
     res = await client.query(
-        QueryOptions(gql(GQL_LISTDATAENTRIES), params)
+        QueryOptions(GQL_OPERATIONS["QUERY_GET_FACTOR"].data, params)
     )
-    # Using the hierarchy approach, we need to check that we have
-    # exactly one user/robot/session in it, otherwise error.
+
+    logger.debug(f"Query result: {res}")
+    # TODO: Check for errors
+    # Using the hierarchy approach, we need to check that we
+    # have exactly one user/robot/session in it, otherwise error.
     if (
         "users" not in res
-        or len(res["users"]) != 1
         or len(res["users"][0]["robots"]) != 1
         or len(res["users"][0]["robots"][0]["sessions"]) != 1
-        or "variables" not in res["users"][0]["robots"][0]["sessions"][0]
+        or "factors" not in res["users"][0]["robots"][0]["sessions"][0]
     ):
-        # Debugging information
-        if len(res["users"]) != 1:
-            logger.warn("User not found in result, returning empty list")
-        if len(res["users"][0]["robots"]) != 1:
-            logger.warn("Robot not found in result, returning empty list")
-        if len(res["users"][0]["robots"][0]["sessions"]) != 1:
-            logger.warn("Robot not found in result, returning empty list")
-        return []
-    
-    # extract result
-    schema = BlobEntrySchema()
-    resdata = res['users'][0]['robots'][0]['sessions'][0]['variables'][0]['data']
-
-    return [
-        schema.load(l) for l in resdata
-    ]
-
-
-async def listDataEntries(
-    client: NavAbilityClient,
-    context: Client,
-    variableLabel,
-):
-    warnings.warn('listDataEntries is deprecated, use listBlobEntries instead.')
-    return await listBlobEntries(client, context, variableLabel)
+        raise Exception(
+            "Received an empty data structure, set logger to debug for the payload"
+        )
+    fs = res["users"][0]["robots"][0]["sessions"][0]["factors"]
+    # TODO: Check for errors
+    if len(fs) == 0:
+        return None
+    if len(fs) > 1:
+        raise Exception(f"More than one factor named {label} returned")
+    if debug:
+        return fs[0]
+    return Factor.load(fs[0])
+
+
+def getFactor(fgclient: DFGClient, label: str, debug=False):
+    tsk = getFactorAsync(fgclient, label, debug=debug)
+    return asyncio.run(tsk)
 
 
+async def listFactorsAsync(fgclient: DFGClient) -> List[str]:
 
+    client = fgclient.client
+    context = fgclient.context
 
-async def addBlobEntry(
-    client: NavAbilityClient,
-    context: Client,
-    variableLabel: str,
-    blobId: str,
-    blobLabel: str,
-    blobSize: int,
-    mimeType: str,
-):
-    """ Add a BlobEntry to a specific variable node in the graph.
-
-    Args:
-        client (NavAbilityClient): client connection to API server
-        context (Client): Unique context with (user, robot, session)
-        variableLabel (string): list data entries connected to which variable.
-        blobId (String): The unique blob identifier of the data.
-        blobLabel (str): blob label.
-        blobSize (int): number of bytes.
-        mimeType (str): standard MIME definition of data.
-
-    Returns:
-        BlobEntry: coroutine 
-    """
     params = {
-        "userId": context.userId,
-        "blobId": blobId,
-        "robotId": context.robotId,
-        "sessionId": context.sessionId,
-        "variableLabel": variableLabel,
-        "blobLabel": blobLabel,
-        "blobSize": blobSize,
-        "mimeType": mimeType,
+        "userLabel": context.userLabel,
+        "robotLabel": context.robotLabel,
+        "sessionLabel": context.sessionLabel,
     }
+
     logger.debug(f"Query params: {params}")
-    res = await client.mutate(
-        MutationOptions(
-            gql(GQL_ADDBLOBENTRY),
-            params,
-        )
+    res = await client.query(
+        QueryOptions(GQL_OPERATIONS["QUERY_LISTFACTORS"].data, params)
     )
-    # TODO error handling
-    # if 'errors' in res:
-    #     raise Exception('Unable to addBlobEntry: '+res['errors'])
-    print(res)
 
-    return res['addBlobEntry']['context']['eventId']
+    logger.debug(f"Query result: {res}")
+    # TODO: Check for errors
+    # Using the hierarchy approach, we need to check that we
+    # have exactly one user/robot/session in it, otherwise error.
+    if (
+        "users" not in res
+        or len(res["users"][0]["robots"]) != 1
+        or len(res["users"][0]["robots"][0]["sessions"]) != 1
+        or "factors" not in res["users"][0]["robots"][0]["sessions"][0]
+    ):
+        raise Exception(
+            "Received an empty data structure, set logger to debug for the payload"
+        )
+    fs = res["users"][0]["robots"][0]["sessions"][0]["factors"]
 
+    fl = []
+    _lb = lambda s: s['label']
+    [fl.append(_lb(f)) for f in fs]
+    return fl
 
-async def addDataEntry(
-    client: NavAbilityClient,
-    context: Client,
-    variableLabel: str,
-    blobId: str,
-    blobLabel: str,
-    blobSize: int,
-    mimeType: str,
-):
-    warnings.warn('addDataEntry is deprecated, use addBlobEntry instead.')
-    return await addBlobEntry(client, context, variableLabel, blobId, blobLabel, blobSize, mimeType)
 
+def listFactors(fgclient: DFGClient):
+    tsk = listFactorsAsync(fgclient)
+    return asyncio.run(tsk)
 
 
-## ==================================
-## download upload blobs
-## ==================================
+# Alias
+lsf = listFactors
 
 
+def assembleFactorName(xisyms: List[str]):
+    s = "".join(xisyms) + "f_" + str(uuid4())[0:4]
+    return s
 
-async def createDownload(
-    client: NavAbilityClient,
-    user: str,
-    blobId: str,
-):
-    """ Request URLs for data blob download.
-
-    Args:
-    client (NavAbilityClient): The NavAbility client for handling requests.
-    userId (String): The userId with access to the data.
-    blobId (String): The unique blob identifier of the data.
-    """
-    params = {
-        "userId": user,
-        "blobId": blobId,
-    }
-    logger.debug(f"Query params: {params}")
-    res = await client.mutate(
-        MutationOptions(
-            gql(GQL_CREATEDOWNLOAD),
-            params,
-        )
-    )
-
-    # TODO error checking
-    if not 'url' in res:
-        raise ValueError('Cannot create download for ', user, " seeking ", blobId)
-    return res['url']
 
+def getFncTypeName(fnc: InferenceType):
+    return type(fnc).__name__
 
 
-async def createUpload(
+async def _addFactorAsync(
     client: NavAbilityClient,
-    blobLabel: str,
-    blobSize: int,
-    parts: int = 1,
+    context: Client,
+    f: Factor,
 ):
-    """ Request URLs for data blob upload.
-
-    Args:
-        client (NavAbilityClient): The NavAbility client.
-        blobLabel (String): human readable blob label (aka filename).
-        filesize (Int): total number of bytes to upload. 
-        parts (Int): Split upload into multiple blob parts, 
-        FIXME currently only supports parts=1.
-
-    Returns:
-        str: The dedicated upload URL
-    """
-    params = {
-        "blobLabel": blobLabel,
-        "blobSize": blobSize,
-        "parts": parts
+    sessionconnect = {
+        "connect": {
+            "where": {
+                "node": {
+                    "label": context.sessionLabel
+                }
+            }
+        }
     }
-    logger.debug(f"Query params: {params}")
-    res = await client.mutate(
-        MutationOptions(
-            gql(GQL_CREATEUPLOAD),
-            params,
-        )
-    )
-    # TODO error handling
-    return res['createUpload']
-
-
 
-async def getBlob(
-    client: NavAbilityClient,
-    user: str,
-    blobId: str,
-):
-    """ If the user has access, retrieve the identified blob of bytes.
-
-    Args:
-        client (NavAbilityClient): The NavAbility client for handling requests.
-        userId (String): The userId with access to the data.
-        blobId (String): The unique blob identifier of the data.
-
-    Returns:
-        data: coroutine with data blob content
-    """
-    url = await createDownload(client, user, blobId)
-    resp = requests.get(url)
-    return resp.content
-
-
-async def getData(
-    client: NavAbilityClient,
-    user: str,
-    blobId: str,
-):
-    warnings.warn('getData is deprecated, use getBlob instead.')
-    return await getBlob(client, user, blobId)
+    variables = {
+        "connect": [
+            {
+                "where": {
+                    "node": {
+                        "sessionConnection": {"node": {"label": context.sessionLabel}},
+                        "label": vlink
+                    }
+                }
+            }
+            for vlink in f._variableOrderSymbols
+        ]
+    }
 
+    factorCreateInput = {
+        'label': f.label,
+        'nstime': f.nstime,
+        'fnctype': f.fnctype,
+        'tags': f.tags,
+        'solvable': f.solvable,
+        'data': FactorSchema().get_data(f),
+        '_variableOrderSymbols': f._variableOrderSymbols,
+        'timestamp': FactorSchema().get_timestamp(f),
+        '_type': f.fnctype,
+        '_version': f._version,
+        'userLabel': context.userLabel,
+        'robotLabel': context.robotLabel,
+        'sessionLabel': context.sessionLabel,
+        'variables': variables,
+        'session': sessionconnect,
+        'metadata': "e30=", #FIXME
+        # 'blobEntries': Optional['FactorBlobEntriesFieldInput'],
+    }
 
+    params = {"factorsToCreate": [factorCreateInput]}
 
-async def completeUploadSingle(
-    client: NavAbilityClient,
-    blobId: str,
-    uploadId: str,
-    eTag: str,
-):
-    #
-    params = {
-        "blobId": blobId,
-        "uploadId": uploadId,
-        "eTag": eTag
-    }
-    logger.debug(f"Query params: {params}")
-    res = await client.mutate(
+    result = await client.mutate(
         MutationOptions(
-            gql(GQL_COMPLETEUPLOAD_SINGLE),
+            GQL_OPERATIONS["MUTATION_ADD_FACTORS"].data,
             params,
         )
     )
-    # TODO error handling
-    return res['completeUpload']
-
-
-
-async def addBlob(
-    client: Client,
-    blobLabel: str,
-    blob
+    #FIXME
+    # return FactorSchema().load(result["addFactors"]["factors"][0])
+    return result["addFactors"]["factors"][0]
+
+
+def addFactorAsync(
+    fgclient: DFGClient,
+    factor_or_labels,
+    fnc=None,
+    multihypo=None,
+    nullhypo=0.0,
+):
+    client = fgclient.client
+    context = fgclient.context
+
+    if isinstance(factor_or_labels, Factor):
+        return _addFactorAsync(client, context, factor_or_labels)
+    elif fnc is not None:
+        fac = Factor(
+            assembleFactorName(factor_or_labels),
+            getFncTypeName(fnc),
+            factor_or_labels,
+            FactorData(
+                fnc=fnc.dump(),
+                multihypo=([] if multihypo is None else multihypo),
+                nullhypo=nullhypo,
+            ),
+        )
+        return _addFactorAsync(client, context, fac)
+    else:
+        raise NotImplementedError()
+
+
+def addFactor(
+    fgclient: DFGClient,
+    factor_or_labels,
+    fnc=None,
+    multihypo=None,
+    nullhypo=0.0,
+):
+    tsk = addFactorAsync(fgclient, factor_or_labels, fnc, multihypo, nullhypo)
+    return asyncio.run(tsk)
+
+
+async def getFactorsAsync(
+    fgclient: DFGClient,
+    # regexFilter: str = ".*",
+    # tags: List[str] = None,
+    # solvable: int = 0,
 ):
-    """Push a data blob to user and get a unique identifier back.
+    client = fgclient.client
+    context = fgclient.context
 
-    Args:
-        client (NavAbilityClient): The NavAbility client for handling requests.
-        blobLabel (str): Human readable label for the blob (aka filename).
-        blob (bytes): Actual data blob as a chunk of data.
-
-    Returns:
-        blobId (String): The unique blob identifier of the data.
-    """
-    blobSize = len(blob)
-    upd = await createUpload(client, blobLabel, blobSize)
-    url = upd['parts'][0]['url']
-    uploadId = upd['uploadId']
-    blobId = upd['file']['id']
-    
-    headers = {
-        'Content-Length': str(blobSize),
-        'Accept': 'application/json, text/plain, */*',
-        'Accept-Encoding': 'gzip, deflate, br',
-        'Sec-Fetch-Dest': 'empty',
-        'Sec-Fetch-Mode': 'cors',
-        'Sec-Fetch-Site': 'cross-site',
-        'Sec-GPC': '1',
-        'Connection': 'keep-alive'
+    params = {
+        "userLabel": context.userLabel,
+        "robotLabel": context.robotLabel,
+        "sessionLabel": context.sessionLabel,
+        # "factor_label_regexp": regexFilter,
+        # "factor_tags": tags if tags is not None else ["FACTOR"],
+        # "solvable": solvable,
+        # "fields_summary": detail in [QueryDetail.SUMMARY, QueryDetail.FULL],
+        # "fields_full": detail == QueryDetail.FULL,
     }
 
-    # do the upload
-    r = requests.put(url, data=blob, headers=headers)
-    
-    # Extract eTag
-    eTag = r.headers['eTag']
-
-    # close out the upload
-    res = await completeUploadSingle(client, blobId, uploadId, eTag)
+    logger.debug(f"Query params: {params}")
+    res = await client.query(
+        QueryOptions(GQL_OPERATIONS["QUERY_GET_FACTORS"].data, params)
+    )
+    logger.debug(f"Query result: {res}")
 
-    return blobId
+    # Using the hierarchy approach, we need to check that
+    # we have exactly one user/robot/session in it, otherwise error.
+    if (
+        "users" not in res
+        or len(res["users"]) != 1
+        or len(res["users"][0]["robots"]) != 1
+        or len(res["users"][0]["robots"][0]["sessions"]) != 1
+        or "factors" not in res["users"][0]["robots"][0]["sessions"][0]
+    ):
+        # Debugging information
+        if len(res["users"]) != 1:
+            logger.warn("User not found in result, returning empty list")
+        if len(res["users"][0]["robots"]) != 1:
+            logger.warn("Robot not found in result, returning empty list")
+        if len(res["users"][0]["robots"][0]["sessions"]) != 1:
+            logger.warn("Robot not found in result, returning empty list")
+        return []
 
+    return [Factor.load(fac) for fac in res["users"][0]["robots"][0]["sessions"][0]["factors"]]
 
 
-async def addData(
-    client: NavAbilityClient,
-    blobLabel: str,
-    blob,
-):
-    warnings.warn('addData is deprecated, use addBlob instead.')
-    return await addBlob(client, blobLabel, blob)
+def getFactors(fgclient: DFGClient):
+    tsk = getFactorsAsync(fgclient)
+    return asyncio.run(tsk)
```

### Comparing `navabilitysdk-0.5.1/src/navability/services/status.py` & `navabilitysdk-0.6.0.post1/src/navability/services/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-from typing import List
+from typing import List, Optional
+import logging
 
 from gql import gql
 
-from navability.common.queries import GQL_GETSTATUSLATEST, GQL_GETSTATUSMESSAGES
+from navability.entities.client import Client
 from navability.entities.navabilityclient import NavAbilityClient, QueryOptions
-from navability.entities.statusmessage import StatusMessageSchema
+from navability.entities.user import User, UserSchema
+from navability.services.loader import GQL_OPERATIONS
 
+logger = logging.getLogger(__name__)
 
-async def getStatusMessages(navAbilityClient: NavAbilityClient, id: str):
-    """Get all the statuses for a request.
 
-    Args:
-        navAbilityClient (NavAbilityClient): The NavAbility client.
-        id (str): The ID of the request that you want the statuses on.
-    """
-    statusMessages = await navAbilityClient.query(
-        QueryOptions(gql(GQL_GETSTATUSMESSAGES), {"id": id})
-    )
-    schema = StatusMessageSchema(many=True)
-    return schema.load(statusMessages["statusMessages"])
-
-
-async def getStatusLatest(navAbilityClient: NavAbilityClient, id: str):
-    """Get the latest status message for a request.
+async def getUsers(navAbilityClient: NavAbilityClient):
+    """Get all users that are accessible by this user.
 
     Args:
         navAbilityClient (NavAbilityClient): The NavAbility client.
-        id (str): The ID of the request that you want the latest status on.
     """
-    statusMessages = await navAbilityClient.query(
-        QueryOptions(gql(GQL_GETSTATUSLATEST), {"id": id})
+    users = await navAbilityClient.query(
+        QueryOptions(GQL_OPERATIONS["QUERY_GET_USERS"].data)
     )
-    schema = StatusMessageSchema()
-    return schema.load(statusMessages["statusLatest"])
+    schema = UserSchema(many=True)
+    return schema.load(users["users"])
 
 
-async def getStatusesLatest(navAbilityClient: NavAbilityClient, ids: List[str]):
-    """Helper function to get a dictionary of all latest statues for a list of results.
+async def getUser(navAbilityClient: NavAbilityClient, userLabel: str) -> Optional[User] :
+    """Get a user.
 
     Args:
         navAbilityClient (NavAbilityClient): The NavAbility client.
-        ids (List[str]): A list of the IDS that you want statuses on.
+        userLabel (str): The email address of the user.
     """
-    return {r: await getStatusLatest(navAbilityClient, r) for r in ids}
+    resp = await navAbilityClient.query(
+        QueryOptions(GQL_OPERATIONS["QUERY_GET_USER"].data, {"userLabel": userLabel})
+    )
+    schema = UserSchema()
+    if len(resp["users"]) != 1:
+        logger.warn(f"No users returned for username ${userLabel}")
+        return None
+    return schema.load(resp["users"][0])
```

### Comparing `navabilitysdk-0.5.1/src/navability/services/variable.py` & `navabilitysdk-0.6.0.post1/src/navability/services/variable.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,100 @@
 import logging
 from typing import List
 
-from gql import gql
+import asyncio
 
-from navability.common.mutations import GQL_ADDVARIABLE
-from navability.common.queries import (
-    GQL_FRAGMENT_VARIABLES,
-    GQL_LISTVARIABLES,
-    GQL_GETVARIABLE,
-    GQL_GETVARIABLES,
-)
+from navability.services.loader import GQL_OPERATIONS
+from navability.entities.dfgclient import DFGClient
 from navability.entities.client import Client
 from navability.entities.navabilityclient import (
     MutationOptions,
     NavAbilityClient,
     QueryOptions,
 )
 from navability.entities.querydetail import QueryDetail
 from navability.entities.variable.variable import (
     Variable,
     VariableSchema,
     VariableSkeleton,
     VariableSkeletonSchema,
+    VariableSummary,
     VariableSummarySchema,
     VariableType,
 )
 
+from navability.entities.variable.ppe import Ppe, PpeSchema
+
+import nest_asyncio
+nest_asyncio.apply()
+
 DETAIL_SCHEMA = {
     QueryDetail.LABEL: None,
     QueryDetail.SKELETON: VariableSkeletonSchema(),
     QueryDetail.SUMMARY: VariableSummarySchema(),
     QueryDetail.FULL: VariableSchema(),
 }
 
 logger = logging.getLogger(__name__)
 
 
-async def _addVariable(navAbilityClient: NavAbilityClient, client: Client, v: Variable):
+async def _addVariableAsync(
+    navAbilityClient: NavAbilityClient,
+    client: Client,
+    v: Variable
+):
+    # {"variable": {"client": client.dump(), "packedData": v.dumpsPacked()}}
+    sessionconnect = {
+        "connect": {
+            "where": {
+                "node": {
+                    "label": client.sessionLabel
+                }
+            }
+        }
+    }
+
+    variableCreateInput = {
+        'label': v.label,
+        'nstime': v.nstime,
+        'variableType': v.variableType,
+        'solvable': v.solvable,
+        'tags': v.tags,
+        '_version': v._version,
+        'timestamp': VariableSchema().get_timestamp(v),
+        'userLabel': client.userLabel,
+        'robotLabel': client.robotLabel,
+        'sessionLabel': client.sessionLabel,
+        'session': sessionconnect,
+        'metadata': "e30=", #FIXME
+        # 'ppes': Optional['VariablePpesFieldInput'],
+        # 'blobEntries': Optional['VariableBlobEntriesFieldInput'],
+        # 'solverData': Optional['VariableSolverDataFieldInput'],
+        # 'factors': Optional['VariableFactorsFieldInput'],
+    }
+
+    params = {"variablesToCreate": [variableCreateInput]}
+
     result = await navAbilityClient.mutate(
         MutationOptions(
-            gql(GQL_ADDVARIABLE),
-            {"variable": {"client": client.dump(), "packedData": v.dumpsPacked()}},
+            GQL_OPERATIONS["MUTATION_ADD_VARIABLES"].data,
+            params,
         )
     )
-    return result["addVariable"]
+    return VariableSchema().load(result["addVariables"]["variables"][0])
+
+
+def _addVariable(navAbilityClient: NavAbilityClient, client: Client, v: Variable):
+    tsk = _addVariableAsync(navAbilityClient, client, v)
+    return asyncio.run(tsk)
 
 
 def addVariable(
-    client: NavAbilityClient, 
-    context: Client, 
-    variable_or_label, 
+    fgclient: DFGClient,
+    variable_or_label,
     varType=None
 ):
     """ Add a variable to the graph.
 
     Args:
         client (NavAbilityClient): client connection to API server
         context (Client): Unique context with (user, robot, session)
@@ -62,53 +103,55 @@
 
     Raises:
         NotImplementedError: _description_
 
     Returns:
         _type_: _description_
     """
+    client = fgclient.client
+    context = fgclient.context
+
     if isinstance(variable_or_label, Variable):
         return _addVariable(client, context, variable_or_label)
     # TODO standardise varType to string or VariableType after design discussion
     if isinstance(varType, str):
         v = Variable(variable_or_label, varType)
         return _addVariable(client, context, v)
     elif isinstance(varType, VariableType):
         v = Variable(variable_or_label, varType.value)
         return _addVariable(client, context, v)
     raise NotImplementedError()
 
 
-async def listVariables(
-    client: NavAbilityClient,
-    context: Client,
+async def listVariablesAsync(
+    fgclient: DFGClient,
     regexFilter: str = ".*",
     tags: List[str] = None,
     solvable: int = 0,
 ) -> List[str]:
-    """Get a list of Variable labels in the graph.
+    """Asynchronous version of listVariables.  Async task returning a string list of Variable labels.
 
     Args:
-        client (NavAbilityClient): client connection to API server
-        context (Client): Unique context with (user, robot, session)
+        fgclient (DFGClient): client connection to API server with unique (user, robot, session) context.
         regexFilter (str, optional): Filter on variable label. Defaults to ".*".
         tags (List[str], optional): Variables can have string tags. Defaults to None.
         solvable (int, optional): Whether this variable can be used in solving yet. Defaults to 0.
-
-    Returns:
-        List[str]: Async task returning a list of Variable labels.
     """
+
+    client = fgclient.client
+    context = fgclient.context
+    
     params = {
-        "userId": context.userId,
-        "robotId": context.robotId,
-        "sessionId": context.sessionId,
+        "userLabel": context.userLabel,
+        "robotLabel": context.robotLabel,
+        "sessionLabel": context.sessionLabel,
     }
     logger.debug(f"Query params: {params}")
     res = await client.query(
-        QueryOptions(gql(GQL_LISTVARIABLES), params)
+        QueryOptions(GQL_OPERATIONS["QUERY_LIST_VARIABLES"].data, params)
     )
     if (
         "users" not in res
         or len(res["users"]) != 1
         or len(res["users"][0]["robots"]) != 1
         or len(res["users"][0]["robots"][0]["sessions"]) != 1
         or "variables" not in res["users"][0]["robots"][0]["sessions"][0]
@@ -122,67 +165,79 @@
             logger.warn("Robot not found in result, returning empty list")
         return []
     vl = []
     _lb = lambda s: s['label']
     resvar = res['users'][0]['robots'][0]['sessions'][0]['variables']
     [vl.append(_lb(v)) for v in resvar]
     return vl
-    # # LEGACY
-    # variables = await getVariables(
-    #     client,
-    #     context,
-    #     detail=QueryDetail.SKELETON,
-    #     regexFilter=regexFilter,
-    #     tags=tags,
-    #     solvable=solvable,
-    # )
-    # result = [v.label for v in variables]
-    # return result
+
+
+def listVariables(
+    fgclient: DFGClient,
+    regexFilter: str = ".*",
+    tags: List[str] = None,
+    solvable: int = 0,
+) -> List[str]:
+    """Returns a string list of Variable labels.
+
+    Args:
+        fgclient (DFGClient): client connection to API server with unique (user, robot, session) context.
+        regexFilter (str, optional): Filter on variable label. Defaults to ".*".
+        tags (List[str], optional): Variables can have string tags. Defaults to None.
+        solvable (int, optional): Whether this variable can be used in solving yet. Defaults to 0.
+    """
+    tsk = listVariablesAsync(fgclient, regexFilter, tags, solvable)
+    return asyncio.run(tsk)
+
+
 
 
 
 # Alias
 ls = listVariables
 
 
-async def getVariables(
-    client: NavAbilityClient,
-    context: Client,
-    detail: QueryDetail = QueryDetail.SKELETON,
+async def getVariablesAsync(
+    fgclient: DFGClient,
+    detail: QueryDetail = QueryDetail.FULL,
     regexFilter: str = ".*",
     tags: List[str] = None,
     solvable: int = 0,
 ) -> List[VariableSkeleton]:
     """Get a list of Variable from a graph using various filters.
 
     Args:
         client (NavAbilityClient): client connection to API server
         context (Client): Unique context with (user, robot, session)
         detail (QueryDetail, optional): Defaults to QueryDetail.SKELETON.
         regexFilter (str, optional): Filter on variable label. Defaults to ".*".
         tags (List[str], optional): Variables can have string tags. Defaults to None.
-        solvable (int, optional): Whether this variable can be used in solving yet. Defaults to 0.
+        solvable (int, optional): Whether this variable can be used in solving yet.
+        Defaults to 0.
 
     Returns:
         List[VariableSkeleton]: Async task returning a list of VariableSkeleton
     """
+
+    client = fgclient.client
+    context = fgclient.context
+
     params = {
-        "userId": context.userId,
-        "robotIds": [context.robotId],
-        "sessionIds": [context.sessionId],
+        "userLabel": context.userLabel,
+        "robotLabel": context.robotLabel,
+        "sessionLabel": context.sessionLabel,
         "variable_label_regexp": regexFilter,
         "variable_tags": tags if tags is not None else ["VARIABLE"],
         "solvable": solvable,
         "fields_summary": detail in [QueryDetail.SUMMARY, QueryDetail.FULL],
         "fields_full": detail == QueryDetail.FULL,
     }
     logger.debug(f"Query params: {params}")
     res = await client.query(
-        QueryOptions(gql(GQL_FRAGMENT_VARIABLES + GQL_GETVARIABLES), params)
-    )
+        QueryOptions(GQL_OPERATIONS["QUERY_GET_VARIABLES"].data, params))
     logger.debug(f"Query result: {res}")
     # TODO: Check for errors
     schema = DETAIL_SCHEMA[detail]
     # Using the hierarchy approach, we need to check that we have
     # exactly one user/robot/session in it, otherwise error.
     if (
         "users" not in res
@@ -202,25 +257,66 @@
     if schema is None:
         return res["users"][0]["robots"][0]["sessions"][0]["variables"]
     return [
         schema.load(l) for l in res["users"][0]["robots"][0]["sessions"][0]["variables"]
     ]
 
 
-async def getVariable(
-    client: NavAbilityClient, 
-    context: Client, 
+def getVariables(
+    fgclient: DFGClient,
+    detail: QueryDetail = QueryDetail.FULL,
+    regexFilter: str = ".*",
+    tags: List[str] = None,
+    solvable: int = 0,
+) -> List[VariableSkeleton]:
+
+    tsk = getVariablesAsync(fgclient, detail, regexFilter, tags, solvable)
+    return asyncio.run(tsk)
+
+
+def getVariablesSummary(
+    fgclient: DFGClient,
+    regexFilter: str = ".*",
+    tags: List[str] = None,
+    solvable: int = 0,
+) -> List[VariableSkeleton]:
+    tsk = getVariablesAsync(fgclient, QueryDetail.SUMMARY, regexFilter, tags, solvable)
+    return asyncio.run(tsk)
+
+
+def getVariablesSkeleton(
+    fgclient: DFGClient,
+    regexFilter: str = ".*",
+    tags: List[str] = None,
+    solvable: int = 0,
+) -> List[VariableSkeleton]:
+    tsk = getVariablesAsync(fgclient, QueryDetail.SKELETON, regexFilter, tags, solvable)
+    return asyncio.run(tsk)
+
+
+async def getVariableAsync(
+    fgclient: DFGClient,
     label: str
 ):
+    """Get a Variable object from the server as connect to via fgclient.
+    
+    :param DFGClient fgclient: connection to servers, containing (user, robot, session) context.
+    :param str label: Variable label to retrieve.
+
+    Returns:
+        Variable: Multilanguage standardized Variable format.
+    """
+    client = fgclient.client
+    context = fgclient.context
+
     params = context.dump()
-    params["label"] = label
+    params["variableLabel"] = label
     logger.debug(f"Query params: {params}")
     res = await client.query(
-        QueryOptions(gql(GQL_FRAGMENT_VARIABLES + GQL_GETVARIABLE), params)
-    )
+        QueryOptions(GQL_OPERATIONS["QUERY_GET_VARIABLE"].data, params))
     logger.debug(f"Query result: {res}")
     # TODO: Check for errors
     # Using the hierarchy approach, we need to check that we have
     # exactly one user/robot/session in it, otherwise error.
     if (
         "users" not in res
         or len(res["users"][0]["robots"]) != 1
@@ -233,7 +329,66 @@
     vs = res["users"][0]["robots"][0]["sessions"][0]["variables"]
     # TODO: Check for errors
     if len(vs) == 0:
         return None
     if len(vs) > 1:
         raise Exception(f"More than one variable named {label} returned")
     return Variable.load(vs[0])
+
+
+def getVariable(
+    fgclient: DFGClient,
+    label: str
+):
+    tsk = getVariableAsync(fgclient, label)
+    return asyncio.run(tsk)
+
+
+# TODO maybe move to seperate ppe.py file
+
+def getPPE(
+    fgclient: DFGClient, 
+    variableLabel: str, 
+    solveKey: str = 'default'
+):
+    client = fgclient.client
+    context = fgclient.context
+
+    params = {
+        "userLabel": context.userLabel,
+        "robotLabel": context.robotLabel,
+        "sessionLabel": context.sessionLabel,
+        "variableLabel": variableLabel,
+        "solveKey": solveKey,
+    }
+    logger.debug(f"Query params: {params}")
+    tsk = client.query(QueryOptions(GQL_OPERATIONS["QUERY_GET_PPE"].data, params))
+    res = asyncio.run(tsk)
+    logger.debug(f"Query result: {res}")
+    # TODO: Check for errors
+    # Using the hierarchy approach, we need to check that we have
+    # exactly one user/robot/session in it, otherwise error.
+    if (
+        "users" not in res
+        or len(res["users"]) != 1
+        or len(res["users"][0]["robots"]) != 1
+        or len(res["users"][0]["robots"][0]["sessions"]) != 1
+        or "variables" not in res["users"][0]["robots"][0]["sessions"][0]
+    ):
+        # Debugging information
+        if len(res["users"]) != 1:
+            logger.warn("User not found in result, returning empty list")
+        if len(res["users"][0]["robots"]) != 1:
+            logger.warn("Robot not found in result, returning empty list")
+        if len(res["users"][0]["robots"][0]["sessions"]) != 1:
+            logger.warn("Robot not found in result, returning empty list")
+        return []
+
+    ppes = res["users"][0]["robots"][0]["sessions"][0]["variables"][0]["ppes"]
+
+    if len(ppes) == 0:
+        return None
+    if len(ppes) > 1:
+        raise Exception(f"More than one variable named {solveKey} returned")
+
+    return Ppe.load(ppes[0])
+
```

### Comparing `navabilitysdk-0.5.1/src/navabilitysdk.egg-info/PKG-INFO` & `navabilitysdk-0.6.0.post1/src/navabilitysdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: navabilitysdk
-Version: 0.5.1
+Version: 0.6.0.post1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: NavAbility
 Author-email: info@navability.io
 License: Apache-2.0
-Download-URL: https://github.com/NavAbility/NavAbilitySDK.py/archive/refs/tags/v0.5.1.tar.gz
+Download-URL: https://github.com/NavAbility/NavAbilitySDK.py/archive/refs/tags/v0.6.0-1.tar.gz
 Description: NavAbility SDK: Access NavAbility Cloud factor graph features from Python.
         Note that this SDK and the related API are in beta. Please let us know if you have any issues at info@navability.io.
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

