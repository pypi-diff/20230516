# Comparing `tmp/simple-wer-0.1.tar.gz` & `tmp/simple-wer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-wer-0.1.tar", last modified: Tue May 16 03:03:54 2023, max compression
+gzip compressed data, was "simple-wer-0.2.tar", last modified: Tue May 16 03:21:29 2023, max compression
```

## Comparing `simple-wer-0.1.tar` & `simple-wer-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 03:03:53.000000 simple-wer-0.1/
--rw-r--r--   0 kangwei   (1092) root         (0)    11357 2023-05-15 04:36:04.000000 simple-wer-0.1/LICENSE
--rw-r--r--   0 kangwei   (1092) root         (0)      659 2023-05-16 03:03:54.000000 simple-wer-0.1/PKG-INFO
--rw-r--r--   0 kangwei   (1092) root         (0)      129 2023-05-15 08:48:32.000000 simple-wer-0.1/README.md
--rw-r--r--   0 kangwei   (1092) root         (0)      775 2023-05-16 03:03:36.000000 simple-wer-0.1/pyproject.toml
--rw-r--r--   0 kangwei   (1092) root         (0)       38 2023-05-16 03:03:53.000000 simple-wer-0.1/setup.cfg
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 03:03:53.000000 simple-wer-0.1/simple_wer/
--rw-r--r--   0 kangwei   (1092) root         (0)      207 2023-05-15 07:22:08.000000 simple-wer-0.1/simple_wer/__init__.py
--rw-r--r--   0 kangwei   (1092) root         (0)     7995 2023-05-15 08:24:37.000000 simple-wer-0.1/simple_wer/simple_wer.py
--rw-r--r--   0 kangwei   (1092) root         (0)      949 2023-05-16 02:57:31.000000 simple-wer-0.1/simple_wer/simple_wer_cli.py
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 03:03:53.000000 simple-wer-0.1/simple_wer.egg-info/
--rw-r--r--   0 kangwei   (1092) root         (0)      659 2023-05-16 03:03:53.000000 simple-wer-0.1/simple_wer.egg-info/PKG-INFO
--rw-r--r--   0 kangwei   (1092) root         (0)      315 2023-05-16 03:03:53.000000 simple-wer-0.1/simple_wer.egg-info/SOURCES.txt
--rw-r--r--   0 kangwei   (1092) root         (0)        1 2023-05-16 03:03:53.000000 simple-wer-0.1/simple_wer.egg-info/dependency_links.txt
--rw-r--r--   0 kangwei   (1092) root         (0)       61 2023-05-16 03:03:53.000000 simple-wer-0.1/simple_wer.egg-info/entry_points.txt
--rw-r--r--   0 kangwei   (1092) root         (0)       22 2023-05-16 03:03:53.000000 simple-wer-0.1/simple_wer.egg-info/requires.txt
--rw-r--r--   0 kangwei   (1092) root         (0)       11 2023-05-16 03:03:53.000000 simple-wer-0.1/simple_wer.egg-info/top_level.txt
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 03:21:28.000000 simple-wer-0.2/
+-rw-r--r--   0 kangwei   (1092) root         (0)    11357 2023-05-15 04:36:04.000000 simple-wer-0.2/LICENSE
+-rw-r--r--   0 kangwei   (1092) root         (0)     2622 2023-05-16 03:21:29.000000 simple-wer-0.2/PKG-INFO
+-rw-r--r--   0 kangwei   (1092) root         (0)     2092 2023-05-16 03:20:54.000000 simple-wer-0.2/README.md
+-rw-r--r--   0 kangwei   (1092) root         (0)      775 2023-05-16 03:21:10.000000 simple-wer-0.2/pyproject.toml
+-rw-r--r--   0 kangwei   (1092) root         (0)       38 2023-05-16 03:21:28.000000 simple-wer-0.2/setup.cfg
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 03:21:28.000000 simple-wer-0.2/simple_wer/
+-rw-r--r--   0 kangwei   (1092) root         (0)      207 2023-05-15 07:22:08.000000 simple-wer-0.2/simple_wer/__init__.py
+-rw-r--r--   0 kangwei   (1092) root         (0)     7995 2023-05-15 08:24:37.000000 simple-wer-0.2/simple_wer/simple_wer.py
+-rw-r--r--   0 kangwei   (1092) root         (0)      949 2023-05-16 02:57:31.000000 simple-wer-0.2/simple_wer/simple_wer_cli.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 03:21:28.000000 simple-wer-0.2/simple_wer.egg-info/
+-rw-r--r--   0 kangwei   (1092) root         (0)     2622 2023-05-16 03:21:28.000000 simple-wer-0.2/simple_wer.egg-info/PKG-INFO
+-rw-r--r--   0 kangwei   (1092) root         (0)      315 2023-05-16 03:21:28.000000 simple-wer-0.2/simple_wer.egg-info/SOURCES.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)        1 2023-05-16 03:21:28.000000 simple-wer-0.2/simple_wer.egg-info/dependency_links.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)       61 2023-05-16 03:21:28.000000 simple-wer-0.2/simple_wer.egg-info/entry_points.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)       22 2023-05-16 03:21:28.000000 simple-wer-0.2/simple_wer.egg-info/requires.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)       11 2023-05-16 03:21:28.000000 simple-wer-0.2/simple_wer.egg-info/top_level.txt
```

### Comparing `simple-wer-0.1/LICENSE` & `simple-wer-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-wer-0.1/pyproject.toml` & `simple-wer-0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-wer"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Wei Kang", email="wkang.pku@gmail.com" },
 ]
 description = "A simple commandline tool for calculating WERs."
 dependencies = [
   "click>=6.7",
   "kaldialign",
```

### Comparing `simple-wer-0.1/simple_wer/simple_wer.py` & `simple-wer-0.2/simple_wer/simple_wer.py`

 * *Files identical despite different names*

### Comparing `simple-wer-0.1/simple_wer/simple_wer_cli.py` & `simple-wer-0.2/simple_wer/simple_wer_cli.py`

 * *Files identical despite different names*

