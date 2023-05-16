# Comparing `tmp/access_nri_intake-0.0.1.tar.gz` & `tmp/access_nri_intake-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_nri_intake-0.0.1.tar", last modified: Tue May 16 02:00:40 2023, max compression
+gzip compressed data, was "access_nri_intake-0.0.2.tar", last modified: Tue May 16 04:26:57 2023, max compression
```

## Comparing `access_nri_intake-0.0.1.tar` & `access_nri_intake-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-sr-x   0 ds0092   (12775) tm70      (8641)        0 2023-05-16 02:00:40.000000 access_nri_intake-0.0.1/
--rw-r--r--   0 ds0092   (12775) tm70      (8641)    11357 2023-03-28 01:32:49.000000 access_nri_intake-0.0.1/LICENSE
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      788 2023-05-16 02:00:40.000000 access_nri_intake-0.0.1/PKG-INFO
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      334 2023-05-11 04:13:35.000000 access_nri_intake-0.0.1/README.md
--rw-r--r--   0 ds0092   (12775) tm70      (8641)     1839 2023-05-16 01:54:46.000000 access_nri_intake-0.0.1/pyproject.toml
--rw-r--r--   0 ds0092   (12775) tm70      (8641)       38 2023-05-16 02:00:40.000000 access_nri_intake-0.0.1/setup.cfg
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      136 2023-05-15 06:10:12.000000 access_nri_intake-0.0.1/setup.py
-drwxr-sr-x   0 ds0092   (12775) tm70      (8641)        0 2023-05-16 02:00:39.000000 access_nri_intake-0.0.1/src/
-drwxr-sr-x   0 ds0092   (12775) tm70      (8641)        0 2023-05-16 02:00:40.000000 access_nri_intake-0.0.1/src/access_nri_intake/
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      373 2023-05-15 10:32:55.000000 access_nri_intake-0.0.1/src/access_nri_intake/__init__.py
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      497 2023-05-16 02:00:40.000000 access_nri_intake-0.0.1/src/access_nri_intake/_version.py
--rw-r--r--   0 ds0092   (12775) tm70      (8641)     4191 2023-05-15 22:48:35.000000 access_nri_intake-0.0.1/src/access_nri_intake/cli.py
-drwxr-sr-x   0 ds0092   (12775) tm70      (8641)        0 2023-05-16 02:00:40.000000 access_nri_intake-0.0.1/src/access_nri_intake/esmcat/
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      710 2023-05-15 22:48:35.000000 access_nri_intake-0.0.1/src/access_nri_intake/esmcat/__init__.py
--rw-r--r--   0 ds0092   (12775) tm70      (8641)    13197 2023-05-16 01:35:16.000000 access_nri_intake-0.0.1/src/access_nri_intake/esmcat/builders.py
--rw-r--r--   0 ds0092   (12775) tm70      (8641)     2889 2023-05-16 01:35:16.000000 access_nri_intake-0.0.1/src/access_nri_intake/esmcat/utils.py
-drwxr-sr-x   0 ds0092   (12775) tm70      (8641)        0 2023-05-16 02:00:40.000000 access_nri_intake-0.0.1/src/access_nri_intake/metacat/
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      931 2023-05-15 22:48:35.000000 access_nri_intake-0.0.1/src/access_nri_intake/metacat/__init__.py
--rw-r--r--   0 ds0092   (12775) tm70      (8641)     6922 2023-05-15 22:48:35.000000 access_nri_intake-0.0.1/src/access_nri_intake/metacat/manager.py
--rw-r--r--   0 ds0092   (12775) tm70      (8641)    10726 2023-05-15 22:48:35.000000 access_nri_intake-0.0.1/src/access_nri_intake/metacat/translators.py
--rw-r--r--   0 ds0092   (12775) tm70      (8641)     3529 2023-05-15 22:48:35.000000 access_nri_intake-0.0.1/src/access_nri_intake/utils.py
-drwxr-sr-x   0 ds0092   (12775) tm70      (8641)        0 2023-05-16 02:00:39.000000 access_nri_intake-0.0.1/src/access_nri_intake.egg-info/
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      788 2023-05-16 02:00:39.000000 access_nri_intake-0.0.1/src/access_nri_intake.egg-info/PKG-INFO
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      703 2023-05-16 02:00:39.000000 access_nri_intake-0.0.1/src/access_nri_intake.egg-info/SOURCES.txt
--rw-r--r--   0 ds0092   (12775) tm70      (8641)        1 2023-05-16 02:00:39.000000 access_nri_intake-0.0.1/src/access_nri_intake.egg-info/dependency_links.txt
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      117 2023-05-16 02:00:39.000000 access_nri_intake-0.0.1/src/access_nri_intake.egg-info/entry_points.txt
--rw-r--r--   0 ds0092   (12775) tm70      (8641)      106 2023-05-16 02:00:39.000000 access_nri_intake-0.0.1/src/access_nri_intake.egg-info/requires.txt
--rw-r--r--   0 ds0092   (12775) tm70      (8641)       18 2023-05-16 02:00:39.000000 access_nri_intake-0.0.1/src/access_nri_intake.egg-info/top_level.txt
--rw-r--r--   0 ds0092   (12775) tm70      (8641)    83751 2023-05-10 05:37:08.000000 access_nri_intake-0.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake/esmcat/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/esmcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/esmcat/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/esmcat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake/metacat/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/metacat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/metacat/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/metacat/translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/metacatalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/src/access_nri_intake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:26:57.541697 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 04:26:57.000000 access_nri_intake-0.0.2/src/access_nri_intake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-16 04:26:43.000000 access_nri_intake-0.0.2/versioneer.py
```

### Comparing `access_nri_intake-0.0.1/LICENSE` & `access_nri_intake-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.1/PKG-INFO` & `access_nri_intake-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_nri_intake
-Version: 0.0.1
+Version: 0.0.2
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.0.1/pyproject.toml` & `access_nri_intake-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,17 @@
   "setuptools >= 61.0.0",
   "versioneer[toml]",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools.package-data]
+access_nri_intake = ["*.yaml"]
+
 [tool.versioneer]
 VCS = "git"
 style = "pep440"
 versionfile_source = "src/access_nri_intake/_version.py"
 versionfile_build = "access_nri_intake/_version.py"
 tag_prefix = "v"
 parentdir_prefix = "access-nri-intake-"
```

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake/cli.py` & `access_nri_intake-0.0.2/src/access_nri_intake/cli.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake/esmcat/__init__.py` & `access_nri_intake-0.0.2/src/access_nri_intake/esmcat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake/esmcat/builders.py` & `access_nri_intake-0.0.2/src/access_nri_intake/esmcat/builders.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake/esmcat/utils.py` & `access_nri_intake-0.0.2/src/access_nri_intake/esmcat/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake/metacat/__init__.py` & `access_nri_intake-0.0.2/src/access_nri_intake/metacat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake/metacat/manager.py` & `access_nri_intake-0.0.2/src/access_nri_intake/metacat/manager.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake/metacat/translators.py` & `access_nri_intake-0.0.2/src/access_nri_intake/metacat/translators.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake/utils.py` & `access_nri_intake-0.0.2/src/access_nri_intake/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake.egg-info/PKG-INFO` & `access_nri_intake-0.0.2/src/access_nri_intake.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-nri-intake
-Version: 0.0.1
+Version: 0.0.2
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.0.1/src/access_nri_intake.egg-info/SOURCES.txt` & `access_nri_intake-0.0.2/src/access_nri_intake.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.py
 versioneer.py
 src/access_nri_intake/__init__.py
 src/access_nri_intake/_version.py
 src/access_nri_intake/cli.py
+src/access_nri_intake/metacatalog.yaml
 src/access_nri_intake/utils.py
 src/access_nri_intake.egg-info/PKG-INFO
 src/access_nri_intake.egg-info/SOURCES.txt
 src/access_nri_intake.egg-info/dependency_links.txt
 src/access_nri_intake.egg-info/entry_points.txt
 src/access_nri_intake.egg-info/requires.txt
 src/access_nri_intake.egg-info/top_level.txt
```

### Comparing `access_nri_intake-0.0.1/versioneer.py` & `access_nri_intake-0.0.2/versioneer.py`

 * *Files identical despite different names*

