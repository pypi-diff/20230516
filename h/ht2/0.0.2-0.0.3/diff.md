# Comparing `tmp/ht2-0.0.2.tar.gz` & `tmp/ht2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht2-0.0.2.tar", last modified: Tue May 16 06:22:23 2023, max compression
+gzip compressed data, was "ht2-0.0.3.tar", last modified: Tue May 16 06:29:58 2023, max compression
```

## Comparing `ht2-0.0.2.tar` & `ht2-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 06:22:23.417356 ht2-0.0.2/
--rw-r--r--   0 agent_h    (501) staff       (20)     1070 2023-05-16 03:28:49.000000 ht2-0.0.2/LICENSE
--rw-r--r--   0 agent_h    (501) staff       (20)      634 2023-05-16 06:22:23.417234 ht2-0.0.2/PKG-INFO
--rw-r--r--   0 agent_h    (501) staff       (20)      126 2023-05-16 06:21:19.000000 ht2-0.0.2/README.md
--rw-r--r--   0 agent_h    (501) staff       (20)      644 2023-05-16 06:16:36.000000 ht2-0.0.2/pyproject.toml
--rw-r--r--   0 agent_h    (501) staff       (20)       38 2023-05-16 06:22:23.417408 ht2-0.0.2/setup.cfg
-drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 06:22:23.414966 ht2-0.0.2/src/
-drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 06:22:23.416233 ht2-0.0.2/src/ht2/
--rw-r--r--   0 agent_h    (501) staff       (20)       23 2023-05-16 06:16:19.000000 ht2-0.0.2/src/ht2/__init__.py
--rw-r--r--   0 agent_h    (501) staff       (20)       71 2023-05-16 03:37:28.000000 ht2-0.0.2/src/ht2/example.py
--rw-r--r--   0 agent_h    (501) staff       (20)      503 2023-05-16 06:16:09.000000 ht2-0.0.2/src/ht2/visualize.py
-drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 06:22:23.417046 ht2-0.0.2/src/ht2.egg-info/
--rw-r--r--   0 agent_h    (501) staff       (20)      634 2023-05-16 06:22:23.000000 ht2-0.0.2/src/ht2.egg-info/PKG-INFO
--rw-r--r--   0 agent_h    (501) staff       (20)      246 2023-05-16 06:22:23.000000 ht2-0.0.2/src/ht2.egg-info/SOURCES.txt
--rw-r--r--   0 agent_h    (501) staff       (20)        1 2023-05-16 06:22:23.000000 ht2-0.0.2/src/ht2.egg-info/dependency_links.txt
--rw-r--r--   0 agent_h    (501) staff       (20)       31 2023-05-16 06:22:23.000000 ht2-0.0.2/src/ht2.egg-info/requires.txt
--rw-r--r--   0 agent_h    (501) staff       (20)        4 2023-05-16 06:22:23.000000 ht2-0.0.2/src/ht2.egg-info/top_level.txt
+drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 06:29:58.567633 ht2-0.0.3/
+-rw-r--r--   0 agent_h    (501) staff       (20)     1070 2023-05-16 03:28:49.000000 ht2-0.0.3/LICENSE
+-rw-r--r--   0 agent_h    (501) staff       (20)      634 2023-05-16 06:29:58.567506 ht2-0.0.3/PKG-INFO
+-rw-r--r--   0 agent_h    (501) staff       (20)      126 2023-05-16 06:21:19.000000 ht2-0.0.3/README.md
+-rw-r--r--   0 agent_h    (501) staff       (20)      644 2023-05-16 06:29:20.000000 ht2-0.0.3/pyproject.toml
+-rw-r--r--   0 agent_h    (501) staff       (20)       38 2023-05-16 06:29:58.567673 ht2-0.0.3/setup.cfg
+drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 06:29:58.565336 ht2-0.0.3/src/
+drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 06:29:58.566519 ht2-0.0.3/src/ht2/
+-rw-r--r--   0 agent_h    (501) staff       (20)       24 2023-05-16 06:25:49.000000 ht2-0.0.3/src/ht2/__init__.py
+-rw-r--r--   0 agent_h    (501) staff       (20)       71 2023-05-16 03:37:28.000000 ht2-0.0.3/src/ht2/example.py
+-rw-r--r--   0 agent_h    (501) staff       (20)      503 2023-05-16 06:16:09.000000 ht2-0.0.3/src/ht2/visualize.py
+drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 06:29:58.567339 ht2-0.0.3/src/ht2.egg-info/
+-rw-r--r--   0 agent_h    (501) staff       (20)      634 2023-05-16 06:29:58.000000 ht2-0.0.3/src/ht2.egg-info/PKG-INFO
+-rw-r--r--   0 agent_h    (501) staff       (20)      246 2023-05-16 06:29:58.000000 ht2-0.0.3/src/ht2.egg-info/SOURCES.txt
+-rw-r--r--   0 agent_h    (501) staff       (20)        1 2023-05-16 06:29:58.000000 ht2-0.0.3/src/ht2.egg-info/dependency_links.txt
+-rw-r--r--   0 agent_h    (501) staff       (20)       31 2023-05-16 06:29:58.000000 ht2-0.0.3/src/ht2.egg-info/requires.txt
+-rw-r--r--   0 agent_h    (501) staff       (20)        4 2023-05-16 06:29:58.000000 ht2-0.0.3/src/ht2.egg-info/top_level.txt
```

### Comparing `ht2-0.0.2/LICENSE` & `ht2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ht2-0.0.2/PKG-INFO` & `ht2-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ht2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Frequently used tools and wrappers for efficiency
 Author-email: Haotian Zhang <z.haotian@columbia.edu>
 Project-URL: Homepage, https://github.com/htplex/ht2
 Project-URL: Bug Tracker, https://github.com/htplex/ht2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ht2-0.0.2/pyproject.toml` & `ht2-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ht2"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Haotian Zhang", email="z.haotian@columbia.edu" },
 ]
 description = "Frequently used tools and wrappers for efficiency"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ht2-0.0.2/src/ht2.egg-info/PKG-INFO` & `ht2-0.0.3/src/ht2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ht2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Frequently used tools and wrappers for efficiency
 Author-email: Haotian Zhang <z.haotian@columbia.edu>
 Project-URL: Homepage, https://github.com/htplex/ht2
 Project-URL: Bug Tracker, https://github.com/htplex/ht2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

