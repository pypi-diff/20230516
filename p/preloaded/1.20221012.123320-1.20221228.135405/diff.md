# Comparing `tmp/preloaded-1.20221012.123320.tar.gz` & `tmp/preloaded-1.20221228.135405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/preloaded-1.20221012.123320.tar", last modified: Wed Oct 12 12:34:31 2022, max compression
+gzip compressed data, was "dist/preloaded-1.20221228.135405.tar", last modified: Wed Dec 28 12:55:24 2022, max compression
```

## Comparing `preloaded-1.20221012.123320.tar` & `preloaded-1.20221228.135405.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5149 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4232 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/preloaded/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/preloaded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/preloaded/_io.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/preloaded/criu.py
--rw-r--r--   0 runner    (1001) docker     (121)     5258 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/preloaded/fork_server.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3335 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/preloaded/py_preloaded_bundle_disk_ckpt.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1656 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/preloaded/py_preloaded_bundle_fork_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/preloaded/startup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/preloaded/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/preloaded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5149 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/preloaded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/preloaded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/preloaded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/preloaded.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/preloaded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-12 12:34:31.000000 preloaded-1.20221012.123320/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4208 2022-10-12 12:34:27.000000 preloaded-1.20221012.123320/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/preloaded/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/preloaded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/preloaded/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/preloaded/criu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/preloaded/fork_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3335 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/preloaded/py_preloaded_bundle_disk_ckpt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1656 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/preloaded/py_preloaded_bundle_fork_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/preloaded/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/preloaded/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/preloaded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/preloaded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/preloaded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/preloaded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/preloaded.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/preloaded.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-28 12:55:24.000000 preloaded-1.20221228.135405/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2022-12-28 12:55:20.000000 preloaded-1.20221228.135405/setup.py
```

### Comparing `preloaded-1.20221012.123320/LICENSE` & `preloaded-1.20221228.135405/LICENSE`

 * *Files identical despite different names*

### Comparing `preloaded-1.20221012.123320/PKG-INFO` & `preloaded-1.20221228.135405/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preloaded
-Version: 1.20221012.123320
+Version: 1.20221228.135405
 Summary: Python Preloaded - Bundle Python executable with preloaded modules
 Home-page: https://github.com/albertz/python-preloaded
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -156,7 +156,10 @@
 However, there is ongoing work to support a non-root option in https://github.com/checkpoint-restore/criu/pull/1930.
 
 Or maybe [DMTCP](https://github.com/dmtcp/dmtcp/) is a better alternative to CRIU?
 
 (Currently incomplete)
 
 
+# Related work
+
+https://github.com/gdb/pyseidon
```

### Comparing `preloaded-1.20221012.123320/README.md` & `preloaded-1.20221228.135405/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -132,7 +132,10 @@
 However, there is ongoing work to support a non-root option in https://github.com/checkpoint-restore/criu/pull/1930.
 
 Or maybe [DMTCP](https://github.com/dmtcp/dmtcp/) is a better alternative to CRIU?
 
 (Currently incomplete)
 
 
+# Related work
+
+https://github.com/gdb/pyseidon
```

### Comparing `preloaded-1.20221012.123320/preloaded/_io.py` & `preloaded-1.20221228.135405/preloaded/_io.py`

 * *Files identical despite different names*

### Comparing `preloaded-1.20221012.123320/preloaded/criu.py` & `preloaded-1.20221228.135405/preloaded/criu.py`

 * *Files identical despite different names*

### Comparing `preloaded-1.20221012.123320/preloaded/fork_server.py` & `preloaded-1.20221228.135405/preloaded/fork_server.py`

 * *Files identical despite different names*

### Comparing `preloaded-1.20221012.123320/preloaded/py_preloaded_bundle_disk_ckpt.py` & `preloaded-1.20221228.135405/preloaded/py_preloaded_bundle_disk_ckpt.py`

 * *Files identical despite different names*

### Comparing `preloaded-1.20221012.123320/preloaded/py_preloaded_bundle_fork_server.py` & `preloaded-1.20221228.135405/preloaded/py_preloaded_bundle_fork_server.py`

 * *Files identical despite different names*

### Comparing `preloaded-1.20221012.123320/preloaded/startup.py` & `preloaded-1.20221228.135405/preloaded/startup.py`

 * *Files identical despite different names*

### Comparing `preloaded-1.20221012.123320/preloaded/utils.py` & `preloaded-1.20221228.135405/preloaded/utils.py`

 * *Files identical despite different names*

### Comparing `preloaded-1.20221012.123320/preloaded.egg-info/PKG-INFO` & `preloaded-1.20221228.135405/preloaded.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preloaded
-Version: 1.20221012.123320
+Version: 1.20221228.135405
 Summary: Python Preloaded - Bundle Python executable with preloaded modules
 Home-page: https://github.com/albertz/python-preloaded
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -156,7 +156,10 @@
 However, there is ongoing work to support a non-root option in https://github.com/checkpoint-restore/criu/pull/1930.
 
 Or maybe [DMTCP](https://github.com/dmtcp/dmtcp/) is a better alternative to CRIU?
 
 (Currently incomplete)
 
 
+# Related work
+
+https://github.com/gdb/pyseidon
```

### Comparing `preloaded-1.20221012.123320/setup.py` & `preloaded-1.20221228.135405/setup.py`

 * *Files identical despite different names*

