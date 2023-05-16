# Comparing `tmp/iguala-0.5.0.tar.gz` & `tmp/iguala-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iguala-0.5.0.tar", last modified: Sat Apr 29 18:48:38 2023, max compression
+gzip compressed data, was "iguala-0.5.1.tar", last modified: Tue May 16 19:31:01 2023, max compression
```

## Comparing `iguala-0.5.0.tar` & `iguala-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:48:38.963733 iguala-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-29 18:48:26.000000 iguala-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-29 18:48:26.000000 iguala-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-29 18:48:26.000000 iguala-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-04-29 18:48:38.963733 iguala-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28431 2023-04-29 18:48:26.000000 iguala-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:48:38.963733 iguala-0.5.0/iguala/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-29 18:48:26.000000 iguala-0.5.0/iguala/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-29 18:48:26.000000 iguala-0.5.0/iguala/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19146 2023-04-29 18:48:26.000000 iguala-0.5.0/iguala/matchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-29 18:48:26.000000 iguala-0.5.0/iguala/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:48:38.963733 iguala-0.5.0/iguala.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-04-29 18:48:38.000000 iguala-0.5.0/iguala.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-29 18:48:38.000000 iguala-0.5.0/iguala.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:48:38.000000 iguala-0.5.0/iguala.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 18:48:38.000000 iguala-0.5.0/iguala.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:48:38.963733 iguala-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-29 18:48:26.000000 iguala-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:31:01.942409 iguala-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-16 19:30:50.000000 iguala-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-16 19:30:50.000000 iguala-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 19:30:50.000000 iguala-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-05-16 19:31:01.942409 iguala-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28431 2023-05-16 19:30:50.000000 iguala-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:31:01.942409 iguala-0.5.1/iguala/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-16 19:30:50.000000 iguala-0.5.1/iguala/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-16 19:30:50.000000 iguala-0.5.1/iguala/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-05-16 19:30:50.000000 iguala-0.5.1/iguala/matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-16 19:30:50.000000 iguala-0.5.1/iguala/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:31:01.942409 iguala-0.5.1/iguala.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-05-16 19:31:01.000000 iguala-0.5.1/iguala.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-16 19:31:01.000000 iguala-0.5.1/iguala.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:31:01.000000 iguala-0.5.1/iguala.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 19:31:01.000000 iguala-0.5.1/iguala.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:31:01.942409 iguala-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-16 19:30:50.000000 iguala-0.5.1/setup.py
```

### Comparing `iguala-0.5.0/CHANGELOG.md` & `iguala-0.5.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # CHANGELOG
 
+## 0.5.1
+
+### Fixes
+
+* Fix issue in the dict matcher, the path were badly interpreted.
+
+
 ## 0.5.0
 
 ### Features
 
 * Add new syntax to describe patterns and matchers
 
 ### Fixes
```

### Comparing `iguala-0.5.0/LICENSE` & `iguala-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iguala-0.5.0/PKG-INFO` & `iguala-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguala
-Version: 0.5.0
+Version: 0.5.1
 Summary: Non-linear pattern matching for Python's objects, or rexep-like for objects
 Home-page: https://github.com/aranega/iguala
 Author: Vincent Aranega
 Author-email: vincent.aranega@gmail.com
 License: BSD 3-Clause
 Keywords: pattern matching matcher regexp graph query term rewriting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iguala-0.5.0/README.md` & `iguala-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `iguala-0.5.0/iguala/helpers.py` & `iguala-0.5.1/iguala/helpers.py`

 * *Files identical despite different names*

### Comparing `iguala-0.5.0/iguala/matchers.py` & `iguala-0.5.1/iguala/matchers.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,17 +260,17 @@
         else:
             props = [(as_path(sl.start), as_matcher(sl.stop)) for sl in properties]
         self._properties = props
 
 
 class DictMatcher(KeyValueMatcher, Matcher):
     def __init__(self, d):
-        self.properties = {
-            as_path(k, dictkey=True): as_matcher(v) for k, v in d.items()
-        }
+        self.properties = [
+            (as_path(k, dictkey=True), as_matcher(v)) for k, v in d.items()
+        ]
 
 
 class LambdaBasedMatcher(Matcher):
     __self__ = "__self__"
 
     def __init__(self, fun):
         self.fun = fun
```

### Comparing `iguala-0.5.0/iguala/paths.py` & `iguala-0.5.1/iguala/paths.py`

 * *Files identical despite different names*

### Comparing `iguala-0.5.0/iguala.egg-info/PKG-INFO` & `iguala-0.5.1/iguala.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguala
-Version: 0.5.0
+Version: 0.5.1
 Summary: Non-linear pattern matching for Python's objects, or rexep-like for objects
 Home-page: https://github.com/aranega/iguala
 Author: Vincent Aranega
 Author-email: vincent.aranega@gmail.com
 License: BSD 3-Clause
 Keywords: pattern matching matcher regexp graph query term rewriting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iguala-0.5.0/setup.py` & `iguala-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if version < (3, 7):
     sys.exit('Sorry, Python < 3.7 is not supported')
 
 packages = ['iguala']
 
 setup(
     name='iguala',
-    version='0.5.0',
+    version='0.5.1',
     description=("Non-linear pattern matching for Python's objects, or rexep-like for objects"),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords='pattern matching matcher regexp graph query term rewriting',
     url='https://github.com/aranega/iguala',
     author='Vincent Aranega',
     author_email='vincent.aranega@gmail.com',
```

