# Comparing `tmp/Plot1Qbit-0.8.tar.gz` & `tmp/Plot1Qbit-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Plot1Qbit-0.8.tar", last modified: Tue Mar 19 19:46:12 2019, max compression
+gzip compressed data, was "dist/Plot1Qbit-0.9.tar", last modified: Tue Mar 19 19:48:48 2019, max compression
```

## Comparing `Plot1Qbit-0.8.tar` & `Plot1Qbit-0.9.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 kmills    (1000) kmills    (1000)        0 2019-03-19 19:46:12.000000 Plot1Qbit-0.8/
--rw-rw-r--   0 kmills    (1000) kmills    (1000)       60 2019-03-19 19:42:17.000000 Plot1Qbit-0.8/MANIFEST.in
--rw-rw-r--   0 kmills    (1000) kmills    (1000)      248 2019-03-19 19:46:12.000000 Plot1Qbit-0.8/PKG-INFO
-drwxrwxr-x   0 kmills    (1000) kmills    (1000)        0 2019-03-19 19:46:12.000000 Plot1Qbit-0.8/Plot1Qbit.egg-info/
--rw-rw-r--   0 kmills    (1000) kmills    (1000)      248 2019-03-19 19:46:12.000000 Plot1Qbit-0.8/Plot1Qbit.egg-info/PKG-INFO
--rw-rw-r--   0 kmills    (1000) kmills    (1000)      206 2019-03-19 19:46:12.000000 Plot1Qbit-0.8/Plot1Qbit.egg-info/SOURCES.txt
--rw-rw-r--   0 kmills    (1000) kmills    (1000)        1 2019-03-19 19:46:12.000000 Plot1Qbit-0.8/Plot1Qbit.egg-info/dependency_links.txt
--rw-rw-r--   0 kmills    (1000) kmills    (1000)       10 2019-03-19 19:46:12.000000 Plot1Qbit-0.8/Plot1Qbit.egg-info/top_level.txt
--rw-rw-r--   0 kmills    (1000) kmills    (1000)      930 2019-03-07 23:06:44.000000 Plot1Qbit-0.8/README.md
-drwxrwxr-x   0 kmills    (1000) kmills    (1000)        0 2019-03-19 19:46:12.000000 Plot1Qbit-0.8/plot1qbit/
--rw-rw-r--   0 kmills    (1000) kmills    (1000)       26 2019-03-07 20:27:49.000000 Plot1Qbit-0.8/plot1qbit/__init__.py
--rw-rw-r--   0 kmills    (1000) kmills    (1000)      384 2019-03-07 20:33:46.000000 Plot1Qbit-0.8/plot1qbit/initiate.py
--rw-rw-r--   0 kmills    (1000) kmills    (1000)       38 2019-03-19 19:46:12.000000 Plot1Qbit-0.8/setup.cfg
--rw-rw-r--   0 kmills    (1000) kmills    (1000)      300 2019-03-19 19:46:05.000000 Plot1Qbit-0.8/setup.py
+drwxrwxr-x   0 kmills    (1000) kmills    (1000)        0 2019-03-19 19:48:48.000000 Plot1Qbit-0.9/
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)       76 2019-03-19 19:48:18.000000 Plot1Qbit-0.9/MANIFEST.in
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)      248 2019-03-19 19:48:48.000000 Plot1Qbit-0.9/PKG-INFO
+drwxrwxr-x   0 kmills    (1000) kmills    (1000)        0 2019-03-19 19:48:48.000000 Plot1Qbit-0.9/Plot1Qbit.egg-info/
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)      248 2019-03-19 19:48:48.000000 Plot1Qbit-0.9/Plot1Qbit.egg-info/PKG-INFO
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)      266 2019-03-19 19:48:48.000000 Plot1Qbit-0.9/Plot1Qbit.egg-info/SOURCES.txt
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)        1 2019-03-19 19:48:48.000000 Plot1Qbit-0.9/Plot1Qbit.egg-info/dependency_links.txt
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)       10 2019-03-19 19:48:48.000000 Plot1Qbit-0.9/Plot1Qbit.egg-info/top_level.txt
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)      930 2019-03-07 23:06:44.000000 Plot1Qbit-0.9/README.md
+drwxrwxr-x   0 kmills    (1000) kmills    (1000)        0 2019-03-19 19:48:48.000000 Plot1Qbit-0.9/plot1qbit/
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)      962 2019-03-07 20:14:22.000000 Plot1Qbit-0.9/plot1qbit/1qbit.mplstyle
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)       26 2019-03-07 20:27:49.000000 Plot1Qbit-0.9/plot1qbit/__init__.py
+-rw-r--r--   0 kmills    (1000) kmills    (1000)    70892 2019-03-07 19:45:09.000000 Plot1Qbit-0.9/plot1qbit/brandon_text_regular.otf
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)      384 2019-03-07 20:33:46.000000 Plot1Qbit-0.9/plot1qbit/initiate.py
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)       38 2019-03-19 19:48:48.000000 Plot1Qbit-0.9/setup.cfg
+-rw-rw-r--   0 kmills    (1000) kmills    (1000)      300 2019-03-19 19:48:44.000000 Plot1Qbit-0.9/setup.py
```

### Comparing `Plot1Qbit-0.8/README.md` & `Plot1Qbit-0.9/README.md`

 * *Files identical despite different names*

