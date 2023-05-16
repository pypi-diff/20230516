# Comparing `tmp/edge-ml-0.2.2.tar.gz` & `tmp/edge-ml-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge-ml-0.2.2.tar", last modified: Thu Sep  1 21:52:05 2022, max compression
+gzip compressed data, was "edge-ml-0.3.tar", last modified: Tue May 16 10:58:14 2023, max compression
```

## Comparing `edge-ml-0.2.2.tar` & `edge-ml-0.3.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 21:52:05.170556 edge-ml-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1075 2022-09-01 21:51:16.000000 edge-ml-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2102 2022-09-01 21:52:05.170556 edge-ml-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1682 2022-09-01 21:51:16.000000 edge-ml-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      352 2022-09-01 21:51:16.000000 edge-ml-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      656 2022-09-01 21:52:05.170556 edge-ml-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 21:52:05.170556 edge-ml-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 21:52:05.170556 edge-ml-0.2.2/src/edge_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2102 2022-09-01 21:52:05.000000 edge-ml-0.2.2/src/edge_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      250 2022-09-01 21:52:05.000000 edge-ml-0.2.2/src/edge_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-01 21:52:05.000000 edge-ml-0.2.2/src/edge_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-09-01 21:52:05.000000 edge-ml-0.2.2/src/edge_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-01 21:52:05.170556 edge-ml-0.2.2/src/edgeml/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-01 21:51:16.000000 edge-ml-0.2.2/src/edgeml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7135 2022-09-01 21:51:16.000000 edge-ml-0.2.2/src/edgeml/edgeml.py
--rw-r--r--   0 runner    (1001) docker     (116)     3536 2022-09-01 21:51:16.000000 edge-ml-0.2.2/src/edgeml/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.467615 edge-ml-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 10:57:53.000000 edge-ml-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-16 10:58:14.467615 edge-ml-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-16 10:57:53.000000 edge-ml-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 10:57:53.000000 edge-ml-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-16 10:58:14.467615 edge-ml-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.463616 edge-ml-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.463616 edge-ml-0.3/src/edge_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-16 10:58:14.000000 edge-ml-0.3/src/edge_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 10:58:14.000000 edge-ml-0.3/src/edge_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:58:14.000000 edge-ml-0.3/src/edge_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 10:58:14.000000 edge-ml-0.3/src/edge_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.463616 edge-ml-0.3/src/edgeml/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/Labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/edgeml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.463616 edge-ml-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-16 10:57:53.000000 edge-ml-0.3/tests/test_predictor.py
```

### Comparing `edge-ml-0.2.2/LICENSE` & `edge-ml-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-ml-0.2.2/setup.cfg` & `edge-ml-0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = edge-ml
-version = 0.2.2
+version = 0.3
 author = KIT/TECO
 autor_email = info@edge-ml.org
 description = Python library of edge-ml.org: end-to-end machine learning for embedded devices
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/edge-ml/python
 project_urls =
```

