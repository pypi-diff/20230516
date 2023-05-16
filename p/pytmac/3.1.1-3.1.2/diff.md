# Comparing `tmp/pytmac-3.1.1.tar.gz` & `tmp/pytmac-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmac-3.1.1.tar", last modified: Tue May 16 20:23:53 2023, max compression
+gzip compressed data, was "pytmac-3.1.2.tar", last modified: Tue May 16 20:26:27 2023, max compression
```

## Comparing `pytmac-3.1.1.tar` & `pytmac-3.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:23:53.640196 pytmac-3.1.1/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-16 20:23:50.000000 pytmac-3.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5028 2023-05-16 20:23:53.636196 pytmac-3.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-16 20:23:50.000000 pytmac-3.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 20:23:50.000000 pytmac-3.1.1/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:23:53.636196 pytmac-3.1.1/bin/
--rw-r--r--   0 root         (0) root         (0)     2719 2023-05-16 20:23:50.000000 pytmac-3.1.1/bin/get_config.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-05-16 20:23:50.000000 pytmac-3.1.1/bin/input_validator.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-05-16 20:23:50.000000 pytmac-3.1.1/bin/resource_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:23:53.636196 pytmac-3.1.1/docs/
--rw-r--r--   0 root         (0) root         (0)      241 2023-05-16 20:23:50.000000 pytmac-3.1.1/docs/config.yaml
--rw-r--r--   0 root         (0) root         (0)     2089 2023-05-16 20:23:50.000000 pytmac-3.1.1/docs/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-16 20:23:50.000000 pytmac-3.1.1/docs/resources.yaml
--rw-r--r--   0 root         (0) root         (0)     7555 2023-05-16 20:23:50.000000 pytmac-3.1.1/docs/security_checks.yaml
--rw-r--r--   0 root         (0) root         (0)     1474 2023-05-16 20:23:50.000000 pytmac-3.1.1/docs/swagger.json
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-16 20:23:50.000000 pytmac-3.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)    18768 2023-05-16 20:23:53.000000 pytmac-3.1.1/pytmac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:23:53.636196 pytmac-3.1.1/pytmac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5028 2023-05-16 20:23:53.000000 pytmac-3.1.1/pytmac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-16 20:23:53.000000 pytmac-3.1.1/pytmac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 20:23:53.000000 pytmac-3.1.1/pytmac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-16 20:23:53.000000 pytmac-3.1.1/pytmac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 20:23:53.000000 pytmac-3.1.1/pytmac.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 20:23:53.640196 pytmac-3.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      868 2023-05-16 20:23:50.000000 pytmac-3.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:26:27.930061 pytmac-3.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-16 20:26:24.000000 pytmac-3.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-05-16 20:26:27.930061 pytmac-3.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4905 2023-05-16 20:26:24.000000 pytmac-3.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 20:26:25.000000 pytmac-3.1.2/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:26:27.930061 pytmac-3.1.2/bin/
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-05-16 20:26:24.000000 pytmac-3.1.2/bin/get_config.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-05-16 20:26:24.000000 pytmac-3.1.2/bin/input_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-05-16 20:26:24.000000 pytmac-3.1.2/bin/resource_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:26:27.930061 pytmac-3.1.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     7555 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/security_checks.yaml
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/swagger.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-16 20:26:24.000000 pytmac-3.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    18768 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:26:27.930061 pytmac-3.1.2/pytmac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 20:26:27.930061 pytmac-3.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      868 2023-05-16 20:26:24.000000 pytmac-3.1.2/setup.py
```

### Comparing `pytmac-3.1.1/LICENSE` & `pytmac-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.1/PKG-INFO` & `pytmac-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmac
-Version: 3.1.1
+Version: 3.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
@@ -57,15 +57,15 @@
 
 To generate an example report based on some pre-defined resources, run the following command:
 
 ```
 pytmac --demo
 ```
 
-This will write to a file called `./reports/report-[today-date].md` which can be viewed in a markdown viewer.
+This will write to a file called `report-[today-date].md` which can be viewed in a markdown viewer.
 
 # Configuration
 
 ## Resources
 
 Resources are defined as any asset that is part of the system being modelled under the following categories:
```

### Comparing `pytmac-3.1.1/README.md` & `pytmac-3.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 To generate an example report based on some pre-defined resources, run the following command:
 
 ```
 pytmac --demo
 ```
 
-This will write to a file called `./reports/report-[today-date].md` which can be viewed in a markdown viewer.
+This will write to a file called `report-[today-date].md` which can be viewed in a markdown viewer.
 
 # Configuration
 
 ## Resources
 
 Resources are defined as any asset that is part of the system being modelled under the following categories:
```

### Comparing `pytmac-3.1.1/bin/get_config.py` & `pytmac-3.1.2/bin/get_config.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.1/bin/input_validator.py` & `pytmac-3.1.2/bin/input_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.1/bin/resource_validator.py` & `pytmac-3.1.2/bin/resource_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.1/docs/defaults.yaml` & `pytmac-3.1.2/docs/defaults.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.1/docs/resources.yaml` & `pytmac-3.1.2/docs/resources.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.1/docs/security_checks.yaml` & `pytmac-3.1.2/docs/security_checks.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.1/docs/swagger.json` & `pytmac-3.1.2/docs/swagger.json`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.1/pytmac` & `pytmac-3.1.2/pytmac`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.1/pytmac.egg-info/PKG-INFO` & `pytmac-3.1.2/pytmac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmac
-Version: 3.1.1
+Version: 3.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
@@ -57,15 +57,15 @@
 
 To generate an example report based on some pre-defined resources, run the following command:
 
 ```
 pytmac --demo
 ```
 
-This will write to a file called `./reports/report-[today-date].md` which can be viewed in a markdown viewer.
+This will write to a file called `report-[today-date].md` which can be viewed in a markdown viewer.
 
 # Configuration
 
 ## Resources
 
 Resources are defined as any asset that is part of the system being modelled under the following categories:
```

### Comparing `pytmac-3.1.1/setup.py` & `pytmac-3.1.2/setup.py`

 * *Files identical despite different names*

