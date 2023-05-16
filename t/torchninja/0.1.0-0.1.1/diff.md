# Comparing `tmp/torchninja-0.1.0.tar.gz` & `tmp/torchninja-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchninja-0.1.0.tar", last modified: Tue May 16 11:21:02 2023, max compression
+gzip compressed data, was "torchninja-0.1.1.tar", last modified: Tue May 16 11:22:29 2023, max compression
```

## Comparing `torchninja-0.1.0.tar` & `torchninja-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:21:02.845134 torchninja-0.1.0/
--rw-r--r--   0 silvan    (1000) silvan    (1000)      590 2023-05-16 11:21:02.845134 torchninja-0.1.0/PKG-INFO
--rw-r--r--   0 silvan    (1000) silvan    (1000)     2119 2023-05-15 13:17:09.000000 torchninja-0.1.0/README.md
--rw-r--r--   0 silvan    (1000) silvan    (1000)       38 2023-05-16 11:21:02.845134 torchninja-0.1.0/setup.cfg
--rw-r--r--   0 silvan    (1000) silvan    (1000)      852 2023-05-15 13:17:59.000000 torchninja-0.1.0/setup.py
-drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:21:02.845134 torchninja-0.1.0/torchninja/
--rw-r--r--   0 silvan    (1000) silvan    (1000)       81 2023-05-16 01:28:51.000000 torchninja-0.1.0/torchninja/__init__.py
-drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:21:02.845134 torchninja-0.1.0/torchninja/core/
--rw-r--r--   0 silvan    (1000) silvan    (1000)        0 2023-05-15 13:12:19.000000 torchninja-0.1.0/torchninja/core/__init__.py
--rw-r--r--   0 silvan    (1000) silvan    (1000)     9556 2023-05-16 01:27:45.000000 torchninja-0.1.0/torchninja/core/trainer.py
--rw-r--r--   0 silvan    (1000) silvan    (1000)      646 2023-05-16 01:28:57.000000 torchninja-0.1.0/torchninja/core/tune.py
-drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:21:02.845134 torchninja-0.1.0/torchninja/core/utils/
--rw-r--r--   0 silvan    (1000) silvan    (1000)        0 2023-05-16 01:26:53.000000 torchninja-0.1.0/torchninja/core/utils/__init__.py
--rw-r--r--   0 silvan    (1000) silvan    (1000)     1825 2023-05-15 19:43:41.000000 torchninja-0.1.0/torchninja/core/utils/logger.py
--rw-r--r--   0 silvan    (1000) silvan    (1000)     4900 2023-05-15 19:43:41.000000 torchninja-0.1.0/torchninja/core/utils/metrics.py
--rw-r--r--   0 silvan    (1000) silvan    (1000)      380 2023-05-15 19:52:25.000000 torchninja-0.1.0/torchninja/core/utils/utils.py
-drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:21:02.845134 torchninja-0.1.0/torchninja/utils/
--rw-r--r--   0 silvan    (1000) silvan    (1000)        0 2023-05-15 11:35:43.000000 torchninja-0.1.0/torchninja/utils/__init__.py
--rw-r--r--   0 silvan    (1000) silvan    (1000)     1102 2023-05-16 01:18:03.000000 torchninja-0.1.0/torchninja/utils/loaders.py
-drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:21:02.845134 torchninja-0.1.0/torchninja.egg-info/
--rw-r--r--   0 silvan    (1000) silvan    (1000)      590 2023-05-16 11:21:02.000000 torchninja-0.1.0/torchninja.egg-info/PKG-INFO
--rw-r--r--   0 silvan    (1000) silvan    (1000)      476 2023-05-16 11:21:02.000000 torchninja-0.1.0/torchninja.egg-info/SOURCES.txt
--rw-r--r--   0 silvan    (1000) silvan    (1000)        1 2023-05-16 11:21:02.000000 torchninja-0.1.0/torchninja.egg-info/dependency_links.txt
--rw-r--r--   0 silvan    (1000) silvan    (1000)       52 2023-05-16 11:21:02.000000 torchninja-0.1.0/torchninja.egg-info/requires.txt
--rw-r--r--   0 silvan    (1000) silvan    (1000)       11 2023-05-16 11:21:02.000000 torchninja-0.1.0/torchninja.egg-info/top_level.txt
+drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:22:29.369284 torchninja-0.1.1/
+-rw-r--r--   0 silvan    (1000) silvan    (1000)     2751 2023-05-16 11:22:29.369284 torchninja-0.1.1/PKG-INFO
+-rw-r--r--   0 silvan    (1000) silvan    (1000)     2119 2023-05-15 13:17:09.000000 torchninja-0.1.1/README.md
+-rw-r--r--   0 silvan    (1000) silvan    (1000)       38 2023-05-16 11:22:29.369284 torchninja-0.1.1/setup.cfg
+-rw-r--r--   0 silvan    (1000) silvan    (1000)     1008 2023-05-16 11:22:26.000000 torchninja-0.1.1/setup.py
+drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:22:29.369284 torchninja-0.1.1/torchninja/
+-rw-r--r--   0 silvan    (1000) silvan    (1000)       81 2023-05-16 01:28:51.000000 torchninja-0.1.1/torchninja/__init__.py
+drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:22:29.369284 torchninja-0.1.1/torchninja/core/
+-rw-r--r--   0 silvan    (1000) silvan    (1000)        0 2023-05-15 13:12:19.000000 torchninja-0.1.1/torchninja/core/__init__.py
+-rw-r--r--   0 silvan    (1000) silvan    (1000)     9556 2023-05-16 01:27:45.000000 torchninja-0.1.1/torchninja/core/trainer.py
+-rw-r--r--   0 silvan    (1000) silvan    (1000)      646 2023-05-16 01:28:57.000000 torchninja-0.1.1/torchninja/core/tune.py
+drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:22:29.369284 torchninja-0.1.1/torchninja/core/utils/
+-rw-r--r--   0 silvan    (1000) silvan    (1000)        0 2023-05-16 01:26:53.000000 torchninja-0.1.1/torchninja/core/utils/__init__.py
+-rw-r--r--   0 silvan    (1000) silvan    (1000)     1825 2023-05-15 19:43:41.000000 torchninja-0.1.1/torchninja/core/utils/logger.py
+-rw-r--r--   0 silvan    (1000) silvan    (1000)     4900 2023-05-15 19:43:41.000000 torchninja-0.1.1/torchninja/core/utils/metrics.py
+-rw-r--r--   0 silvan    (1000) silvan    (1000)      380 2023-05-15 19:52:25.000000 torchninja-0.1.1/torchninja/core/utils/utils.py
+drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:22:29.369284 torchninja-0.1.1/torchninja/utils/
+-rw-r--r--   0 silvan    (1000) silvan    (1000)        0 2023-05-15 11:35:43.000000 torchninja-0.1.1/torchninja/utils/__init__.py
+-rw-r--r--   0 silvan    (1000) silvan    (1000)     1102 2023-05-16 01:18:03.000000 torchninja-0.1.1/torchninja/utils/loaders.py
+drwxr-xr-x   0 silvan    (1000) silvan    (1000)        0 2023-05-16 11:22:29.369284 torchninja-0.1.1/torchninja.egg-info/
+-rw-r--r--   0 silvan    (1000) silvan    (1000)     2751 2023-05-16 11:22:29.000000 torchninja-0.1.1/torchninja.egg-info/PKG-INFO
+-rw-r--r--   0 silvan    (1000) silvan    (1000)      476 2023-05-16 11:22:29.000000 torchninja-0.1.1/torchninja.egg-info/SOURCES.txt
+-rw-r--r--   0 silvan    (1000) silvan    (1000)        1 2023-05-16 11:22:29.000000 torchninja-0.1.1/torchninja.egg-info/dependency_links.txt
+-rw-r--r--   0 silvan    (1000) silvan    (1000)       52 2023-05-16 11:22:29.000000 torchninja-0.1.1/torchninja.egg-info/requires.txt
+-rw-r--r--   0 silvan    (1000) silvan    (1000)       11 2023-05-16 11:22:29.000000 torchninja-0.1.1/torchninja.egg-info/top_level.txt
```

### Comparing `torchninja-0.1.0/README.md` & `torchninja-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `torchninja-0.1.0/torchninja/core/trainer.py` & `torchninja-0.1.1/torchninja/core/trainer.py`

 * *Files identical despite different names*

### Comparing `torchninja-0.1.0/torchninja/core/tune.py` & `torchninja-0.1.1/torchninja/core/tune.py`

 * *Files identical despite different names*

### Comparing `torchninja-0.1.0/torchninja/core/utils/logger.py` & `torchninja-0.1.1/torchninja/core/utils/logger.py`

 * *Files identical despite different names*

### Comparing `torchninja-0.1.0/torchninja/core/utils/metrics.py` & `torchninja-0.1.1/torchninja/core/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `torchninja-0.1.0/torchninja/utils/loaders.py` & `torchninja-0.1.1/torchninja/utils/loaders.py`

 * *Files identical despite different names*

