# Comparing `tmp/borg_space-1.0.tar.gz` & `tmp/borg_space-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borg_space-1.0.tar", last modified: Sun Apr  9 05:02:50 2023, max compression
+gzip compressed data, was "borg_space-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `borg_space-1.0.tar` & `borg_space-2.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-10-22 21:26:19.370225 borg_space-1.0/LICENSE
--rw-r--r--   0        0        0     3693 2023-04-09 04:39:15.072813 borg_space-1.0/README.rst
--rwxr-xr-x   0        0        0     6651 2023-04-09 04:38:00.405766 borg_space-1.0/borg_space.py
--rw-r--r--   0        0        0     1362 2023-04-09 04:47:40.123167 borg_space-1.0/pyproject.toml
--rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 borg_space-1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-22 21:26:19.370225 borg_space-2.0/LICENSE
+-rw-r--r--   0        0        0     8785 2023-05-16 05:57:30.537517 borg_space-2.0/README.rst
+-rw-r--r--   0        0        0        0 2023-05-05 05:24:18.834041 borg_space-2.0/borg_space/__init__.py
+-rw-r--r--   0        0        0     6943 2023-05-16 04:24:30.512097 borg_space-2.0/borg_space/config.py
+-rw-r--r--   0        0        0    10680 2023-05-16 05:57:30.536517 borg_space-2.0/borg_space/main.py
+-rw-r--r--   0        0        0     2978 2023-05-16 04:26:51.372451 borg_space-2.0/borg_space/trees.py
+-rw-r--r--   0        0        0     1183 2023-05-16 05:57:30.535517 borg_space-2.0/pyproject.toml
+-rw-r--r--   0        0        0     9842 1970-01-01 00:00:00.000000 borg_space-2.0/PKG-INFO
```

### Comparing `borg_space-1.0/LICENSE` & `borg_space-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `borg_space-1.0/pyproject.toml` & `borg_space-2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 [project]
 name = "borg_space"
 dist-name = "borg-space"
-version = "1.0"
+version = "2.0"
 description = "Accessory for Emborg used to report and track the size of your Borg repositories"
 readme = "README.rst"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 keywords = ["emborg", "borg", "backups"]
 authors = [{name = "Ken Kundert", email = "emborg@nurdletech.com"}]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Natural Language :: English",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3",
     "Topic :: Utilities",
 ]
 dependencies = [
     "appdirs",
-    "arrow>=0.15",
+    "arrow",
     "docopt",
-    "emborg>=1.31",
-    "inform>=1.26",
+    "inform",
     "matplotlib",
     "nestedtext",
     "quantiphy",
+    "shlib",
+    "voluptuous",
 ]
 
 [project.urls]
 homepage = "https://github.com/kenkundert/borg-space"
 repository = "https://github.com/kenkundert/borg-space"
 documentation = "https://github.com/KenKundert/borg-space/blob/master/README.rst"
 changelog = "https://github.com/KenKundert/ntlog/blob/master/CHANGELOG.rst"
 
 [project.scripts]
-borg-space = "borg_space:main"
+borg-space = "borg_space.main:main"
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

