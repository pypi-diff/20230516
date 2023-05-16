# Comparing `tmp/yambs-0.1.0.tar.gz` & `tmp/yambs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-0.1.0.tar", last modified: Mon May 15 08:38:19 2023, max compression
+gzip compressed data, was "yambs-1.0.0.tar", last modified: Tue May 16 08:31:13 2023, max compression
```

## Comparing `yambs-0.1.0.tar` & `yambs-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:38:19.571477 yambs-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 08:37:18.000000 yambs-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-15 08:38:19.571477 yambs-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-15 08:37:18.000000 yambs-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-15 08:37:18.000000 yambs-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 08:38:19.571477 yambs-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-15 08:37:18.000000 yambs-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:38:19.571477 yambs-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 08:37:18.000000 yambs-0.1.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-15 08:37:18.000000 yambs-0.1.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:38:19.571477 yambs-0.1.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-15 08:37:18.000000 yambs-0.1.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-15 08:37:18.000000 yambs-0.1.0/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-15 08:37:18.000000 yambs-0.1.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:38:19.571477 yambs-0.1.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:37:18.000000 yambs-0.1.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-15 08:37:18.000000 yambs-0.1.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 08:37:18.000000 yambs-0.1.0/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-15 08:37:18.000000 yambs-0.1.0/yambs/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:37:18.000000 yambs-0.1.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 08:37:18.000000 yambs-0.1.0/yambs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:38:19.571477 yambs-0.1.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-15 08:38:19.000000 yambs-0.1.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 08:38:19.000000 yambs-0.1.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:38:19.000000 yambs-0.1.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 08:38:19.000000 yambs-0.1.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 08:38:19.000000 yambs-0.1.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 08:38:19.000000 yambs-0.1.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 08:30:07.000000 yambs-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-16 08:31:13.057013 yambs-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-05-16 08:30:07.000000 yambs-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-16 08:30:07.000000 yambs-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:31:13.057013 yambs-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-16 08:30:07.000000 yambs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.053013 yambs-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 08:30:07.000000 yambs-1.0.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-16 08:30:07.000000 yambs-1.0.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.053013 yambs-1.0.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.053013 yambs-1.0.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-16 08:30:07.000000 yambs-1.0.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:31:13.057013 yambs-1.0.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 08:31:13.000000 yambs-1.0.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-0.1.0/LICENSE` & `yambs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-0.1.0/pyproject.toml` & `yambs-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "0.1.0"
+version = "1.0.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Unix",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License"
 ]
```

### Comparing `yambs-0.1.0/setup.py` & `yambs-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=c1a678ba417e2f305577865f259988da
+# hash=ce6be60164e81cbf11eb963d361db255
 # =====================================
 
 """
 yambs - Package definition for distribution.
 """
 
 # third-party
@@ -28,13 +28,14 @@
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
         "3.7",
         "3.8",
         "3.9",
         "3.10",
+        "3.11",
     ],
 }
 setup(
     pkg_info,
     author_info,
 )
```

### Comparing `yambs-0.1.0/tests/test_entry.py` & `yambs-1.0.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-0.1.0/yambs/app.py` & `yambs-1.0.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-0.1.0/yambs/entry.py` & `yambs-1.0.0/yambs/entry.py`

 * *Files identical despite different names*

