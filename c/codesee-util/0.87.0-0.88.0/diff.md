# Comparing `tmp/codesee-util-0.87.0.tar.gz` & `tmp/codesee-util-0.88.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/cubes/codesee/codesee/python/codesee-util/dist/tmpfjkt6rcu/codesee-util-0.87.0.tar", last modified: Wed Sep 15 21:05:26 2021, max compression
+gzip compressed data, was "codesee-util-0.88.0.tar", last modified: Tue May 16 18:29:40 2023, max compression
```

## Comparing `codesee-util-0.87.0.tar` & `codesee-util-0.88.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 cubes      (501) staff       (20)        0 2021-09-15 21:05:26.000000 codesee-util-0.87.0/
--rw-r--r--   0 cubes      (501) staff       (20)      510 2021-09-09 22:16:26.000000 codesee-util-0.87.0/LICENSE
--rw-r--r--   0 cubes      (501) staff       (20)      822 2021-09-15 21:05:26.000000 codesee-util-0.87.0/PKG-INFO
--rw-r--r--   0 cubes      (501) staff       (20)      317 2021-09-09 22:16:26.000000 codesee-util-0.87.0/README.md
--rw-r--r--   0 cubes      (501) staff       (20)      104 2021-09-09 22:16:26.000000 codesee-util-0.87.0/pyproject.toml
--rw-r--r--   0 cubes      (501) staff       (20)      766 2021-09-15 21:05:26.000000 codesee-util-0.87.0/setup.cfg
-drwxr-xr-x   0 cubes      (501) staff       (20)        0 2021-09-15 21:05:26.000000 codesee-util-0.87.0/src/
-drwxr-xr-x   0 cubes      (501) staff       (20)        0 2021-09-15 21:05:26.000000 codesee-util-0.87.0/src/codesee_util/
--rw-r--r--   0 cubes      (501) staff       (20)       70 2021-09-15 20:44:10.000000 codesee-util-0.87.0/src/codesee_util/__init__.py
--rwxr-xr-x   0 cubes      (501) staff       (20)     1042 2021-09-09 22:16:26.000000 codesee-util-0.87.0/src/codesee_util/cli.py
--rwxr-xr-x   0 cubes      (501) staff       (20)     5353 2021-09-09 22:16:26.000000 codesee-util-0.87.0/src/codesee_util/package_info.py
-drwxr-xr-x   0 cubes      (501) staff       (20)        0 2021-09-15 21:05:26.000000 codesee-util-0.87.0/src/codesee_util.egg-info/
--rw-r--r--   0 cubes      (501) staff       (20)      822 2021-09-15 21:05:25.000000 codesee-util-0.87.0/src/codesee_util.egg-info/PKG-INFO
--rw-r--r--   0 cubes      (501) staff       (20)      370 2021-09-15 21:05:26.000000 codesee-util-0.87.0/src/codesee_util.egg-info/SOURCES.txt
--rw-r--r--   0 cubes      (501) staff       (20)        1 2021-09-15 21:05:25.000000 codesee-util-0.87.0/src/codesee_util.egg-info/dependency_links.txt
--rw-r--r--   0 cubes      (501) staff       (20)       54 2021-09-15 21:05:25.000000 codesee-util-0.87.0/src/codesee_util.egg-info/entry_points.txt
--rw-r--r--   0 cubes      (501) staff       (20)       32 2021-09-15 21:05:25.000000 codesee-util-0.87.0/src/codesee_util.egg-info/requires.txt
--rw-r--r--   0 cubes      (501) staff       (20)       13 2021-09-15 21:05:25.000000 codesee-util-0.87.0/src/codesee_util.egg-info/top_level.txt
+drwxr-xr-x   0 cubes      (501) staff       (20)        0 2023-05-16 18:29:40.707593 codesee-util-0.88.0/
+-rw-r--r--   0 cubes      (501) staff       (20)      510 2021-09-09 22:16:26.000000 codesee-util-0.88.0/LICENSE
+-rw-r--r--   0 cubes      (501) staff       (20)      785 2023-05-16 18:29:40.707896 codesee-util-0.88.0/PKG-INFO
+-rw-r--r--   0 cubes      (501) staff       (20)      317 2021-09-09 22:16:26.000000 codesee-util-0.88.0/README.md
+-rw-r--r--   0 cubes      (501) staff       (20)      104 2021-09-09 22:16:26.000000 codesee-util-0.88.0/pyproject.toml
+-rw-r--r--   0 cubes      (501) staff       (20)      774 2023-05-16 18:29:40.708952 codesee-util-0.88.0/setup.cfg
+drwxr-xr-x   0 cubes      (501) staff       (20)        0 2023-05-16 18:29:40.700720 codesee-util-0.88.0/src/
+drwxr-xr-x   0 cubes      (501) staff       (20)        0 2023-05-16 18:29:40.704399 codesee-util-0.88.0/src/codesee_util/
+-rw-r--r--   0 cubes      (501) staff       (20)       70 2023-05-16 18:29:18.000000 codesee-util-0.88.0/src/codesee_util/__init__.py
+-rwxr-xr-x   0 cubes      (501) staff       (20)     1042 2021-09-09 22:16:26.000000 codesee-util-0.88.0/src/codesee_util/cli.py
+-rwxr-xr-x   0 cubes      (501) staff       (20)     5353 2021-09-09 22:16:26.000000 codesee-util-0.88.0/src/codesee_util/package_info.py
+drwxr-xr-x   0 cubes      (501) staff       (20)        0 2023-05-16 18:29:40.707253 codesee-util-0.88.0/src/codesee_util.egg-info/
+-rw-r--r--   0 cubes      (501) staff       (20)      785 2023-05-16 18:29:40.000000 codesee-util-0.88.0/src/codesee_util.egg-info/PKG-INFO
+-rw-r--r--   0 cubes      (501) staff       (20)      370 2023-05-16 18:29:40.000000 codesee-util-0.88.0/src/codesee_util.egg-info/SOURCES.txt
+-rw-r--r--   0 cubes      (501) staff       (20)        1 2023-05-16 18:29:40.000000 codesee-util-0.88.0/src/codesee_util.egg-info/dependency_links.txt
+-rw-r--r--   0 cubes      (501) staff       (20)       53 2023-05-16 18:29:40.000000 codesee-util-0.88.0/src/codesee_util.egg-info/entry_points.txt
+-rw-r--r--   0 cubes      (501) staff       (20)       40 2023-05-16 18:29:40.000000 codesee-util-0.88.0/src/codesee_util.egg-info/requires.txt
+-rw-r--r--   0 cubes      (501) staff       (20)       13 2023-05-16 18:29:40.000000 codesee-util-0.88.0/src/codesee_util.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `codesee-util-0.87.0/PKG-INFO` & `codesee-util-0.88.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: codesee-util
-Version: 0.87.0
+Version: 0.88.0
 Summary: CodeSee Python utilities
 Home-page: https://www.codesee.io
 Author: CodeSee
 Author-email: cubes@codesee.io
-License: UNKNOWN
 Keywords: CodeSee,continuous,understanding
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pydeps
 License-File: LICENSE
@@ -22,9 +20,7 @@
 [CodeSee](https://www.codesee.io). Includes the following:
 
 ## codesee-py
 
 A command-line utility we use when generating CodeSee Maps. It
 has the ability to introspect a directory containing a Python package,
 and emits information about that package.
-
-
```

### Comparing `codesee-util-0.87.0/setup.cfg` & `codesee-util-0.88.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 python_requires = >=3.6
 
 [options.entry_points]
 console_scripts = 
 	codesee-py = codesee_util.cli:main
 
 [options.extras_require]
-pydeps = pydeps
+pydeps = pydeps<=1.12.4
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `codesee-util-0.87.0/src/codesee_util/cli.py` & `codesee-util-0.88.0/src/codesee_util/cli.py`

 * *Files identical despite different names*

### Comparing `codesee-util-0.87.0/src/codesee_util/package_info.py` & `codesee-util-0.88.0/src/codesee_util/package_info.py`

 * *Files identical despite different names*

### Comparing `codesee-util-0.87.0/src/codesee_util.egg-info/PKG-INFO` & `codesee-util-0.88.0/src/codesee_util.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: codesee-util
-Version: 0.87.0
+Version: 0.88.0
 Summary: CodeSee Python utilities
 Home-page: https://www.codesee.io
 Author: CodeSee
 Author-email: cubes@codesee.io
-License: UNKNOWN
 Keywords: CodeSee,continuous,understanding
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pydeps
 License-File: LICENSE
@@ -22,9 +20,7 @@
 [CodeSee](https://www.codesee.io). Includes the following:
 
 ## codesee-py
 
 A command-line utility we use when generating CodeSee Maps. It
 has the ability to introspect a directory containing a Python package,
 and emits information about that package.
-
-
```

