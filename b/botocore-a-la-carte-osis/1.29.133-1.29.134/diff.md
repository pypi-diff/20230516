# Comparing `tmp/botocore-a-la-carte-osis-1.29.133.tar.gz` & `tmp/botocore-a-la-carte-osis-1.29.134.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-osis-1.29.133.tar", last modified: Sat May 13 01:14:22 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-osis-1.29.134.tar", last modified: Tue May 16 01:18:01 2023, max compression
```

## Comparing `botocore-a-la-carte-osis-1.29.133.tar` & `botocore-a-la-carte-osis-1.29.134.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:14:22.881805 botocore-a-la-carte-osis-1.29.133/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-13 01:14:22.000000 botocore-a-la-carte-osis-1.29.133/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-13 01:14:22.881805 botocore-a-la-carte-osis-1.29.133/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:14:22.877805 botocore-a-la-carte-osis-1.29.133/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:14:22.877805 botocore-a-la-carte-osis-1.29.133/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:14:22.877805 botocore-a-la-carte-osis-1.29.133/botocore/data/osis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:14:22.881805 botocore-a-la-carte-osis-1.29.133/botocore/data/osis/2022-01-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-05-13 01:13:41.000000 botocore-a-la-carte-osis-1.29.133/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 01:13:41.000000 botocore-a-la-carte-osis-1.29.133/botocore/data/osis/2022-01-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-05-13 01:13:41.000000 botocore-a-la-carte-osis-1.29.133/botocore/data/osis/2022-01-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:14:22.881805 botocore-a-la-carte-osis-1.29.133/botocore_a_la_carte_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-13 01:14:22.000000 botocore-a-la-carte-osis-1.29.133/botocore_a_la_carte_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-13 01:14:22.000000 botocore-a-la-carte-osis-1.29.133/botocore_a_la_carte_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 01:14:22.000000 botocore-a-la-carte-osis-1.29.133/botocore_a_la_carte_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-13 01:14:22.000000 botocore-a-la-carte-osis-1.29.133/botocore_a_la_carte_osis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 01:14:22.881805 botocore-a-la-carte-osis-1.29.133/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-13 01:14:22.000000 botocore-a-la-carte-osis-1.29.133/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:01.952883 botocore-a-la-carte-osis-1.29.134/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-16 01:18:01.000000 botocore-a-la-carte-osis-1.29.134/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-16 01:18:01.952883 botocore-a-la-carte-osis-1.29.134/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:01.952883 botocore-a-la-carte-osis-1.29.134/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:01.952883 botocore-a-la-carte-osis-1.29.134/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:01.952883 botocore-a-la-carte-osis-1.29.134/botocore/data/osis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:01.952883 botocore-a-la-carte-osis-1.29.134/botocore/data/osis/2022-01-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-05-16 01:17:26.000000 botocore-a-la-carte-osis-1.29.134/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 01:17:26.000000 botocore-a-la-carte-osis-1.29.134/botocore/data/osis/2022-01-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-05-16 01:17:26.000000 botocore-a-la-carte-osis-1.29.134/botocore/data/osis/2022-01-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:01.952883 botocore-a-la-carte-osis-1.29.134/botocore_a_la_carte_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-16 01:18:01.000000 botocore-a-la-carte-osis-1.29.134/botocore_a_la_carte_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-16 01:18:01.000000 botocore-a-la-carte-osis-1.29.134/botocore_a_la_carte_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:18:01.000000 botocore-a-la-carte-osis-1.29.134/botocore_a_la_carte_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 01:18:01.000000 botocore-a-la-carte-osis-1.29.134/botocore_a_la_carte_osis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 01:18:01.952883 botocore-a-la-carte-osis-1.29.134/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 01:18:01.000000 botocore-a-la-carte-osis-1.29.134/setup.py
```

### Comparing `botocore-a-la-carte-osis-1.29.133/LICENSE.txt` & `botocore-a-la-carte-osis-1.29.134/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-osis-1.29.133/PKG-INFO` & `botocore-a-la-carte-osis-1.29.134/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-osis
-Version: 1.29.133
+Version: 1.29.134
 Summary: osis data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-osis-1.29.133/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-osis-1.29.134/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-osis-1.29.133/botocore/data/osis/2022-01-01/service-2.json` & `botocore-a-la-carte-osis-1.29.134/botocore/data/osis/2022-01-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-osis-1.29.133/botocore_a_la_carte_osis.egg-info/PKG-INFO` & `botocore-a-la-carte-osis-1.29.134/botocore_a_la_carte_osis.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-osis
-Version: 1.29.133
+Version: 1.29.134
 Summary: osis data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-osis-1.29.133/setup.py` & `botocore-a-la-carte-osis-1.29.134/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-osis',
-    version="1.29.133",
+    version="1.29.134",
     description='osis data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/osis/*/*.json'],
```

