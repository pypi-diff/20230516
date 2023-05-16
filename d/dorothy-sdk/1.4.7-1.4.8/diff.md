# Comparing `tmp/dorothy-sdk-1.4.7.tar.gz` & `tmp/dorothy-sdk-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorothy-sdk-1.4.7.tar", last modified: Thu May 11 13:08:17 2023, max compression
+gzip compressed data, was "dorothy-sdk-1.4.8.tar", last modified: Tue May 16 21:52:04 2023, max compression
```

## Comparing `dorothy-sdk-1.4.7.tar` & `dorothy-sdk-1.4.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.251549 dorothy-sdk-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-11 13:08:17.251549 dorothy-sdk-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.251549 dorothy-sdk-1.4.7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6021 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/bin/model_run
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/bin/model_train
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.247549 dorothy-sdk-1.4.7/dorothy_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.247549 dorothy-sdk-1.4.7/dorothy_sdk/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/resources/quality_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/dorothy_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:08:17.247549 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 13:08:17.000000 dorothy-sdk-1.4.7/dorothy_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:08:17.251549 dorothy-sdk-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-11 13:08:03.000000 dorothy-sdk-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:04.313543 dorothy-sdk-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-16 21:52:04.313543 dorothy-sdk-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:04.313543 dorothy-sdk-1.4.8/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6021 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/bin/model_run
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/bin/model_train
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:04.309543 dorothy-sdk-1.4.8/dorothy_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:04.313543 dorothy-sdk-1.4.8/dorothy_sdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/resources/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/resources/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/resources/folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/resources/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/resources/quality_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/dorothy_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:04.313543 dorothy-sdk-1.4.8/dorothy_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-16 21:52:04.000000 dorothy-sdk-1.4.8/dorothy_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-16 21:52:04.000000 dorothy-sdk-1.4.8/dorothy_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:52:04.000000 dorothy-sdk-1.4.8/dorothy_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 21:52:04.000000 dorothy-sdk-1.4.8/dorothy_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 21:52:04.000000 dorothy-sdk-1.4.8/dorothy_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:52:04.313543 dorothy-sdk-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-16 21:51:47.000000 dorothy-sdk-1.4.8/setup.py
```

### Comparing `dorothy-sdk-1.4.7/PKG-INFO` & `dorothy-sdk-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorothy-sdk
-Version: 1.4.7
+Version: 1.4.8
 Summary: UNKNOWN
 Home-page: https://github.com/tb-brics/dorothy-sdk
 Author: Patrick Braz
 Author-email: patrickfbraz@poli.ufrj.br
 Maintainer: Patrick Braz
 Maintainer-email: patrickfbraz@poli.ufrj.br
 License: UNKNOWN
```

### Comparing `dorothy-sdk-1.4.7/README.rst` & `dorothy-sdk-1.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/bin/model_run` & `dorothy-sdk-1.4.8/bin/model_run`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/bin/model_train` & `dorothy-sdk-1.4.8/bin/model_train`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/core.py` & `dorothy-sdk-1.4.8/dorothy_sdk/core.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/dataset_wrapper.py` & `dorothy-sdk-1.4.8/dorothy_sdk/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/git_repo.py` & `dorothy-sdk-1.4.8/dorothy_sdk/git_repo.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/mlflow.py` & `dorothy-sdk-1.4.8/dorothy_sdk/mlflow.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/operation.py` & `dorothy-sdk-1.4.8/dorothy_sdk/operation.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/resources/dataset.py` & `dorothy-sdk-1.4.8/dorothy_sdk/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/resources/folders.py` & `dorothy-sdk-1.4.8/dorothy_sdk/resources/folders.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/resources/folds.py` & `dorothy-sdk-1.4.8/dorothy_sdk/resources/folds.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 row["project_id"] = image.project_id
                 row["target"] = image.has_tb
                 row["role"] = "VAL"
                 row["dataset_name"] = image.dataset_name
                 yield row
 
     def get_pandas_dataframe(self):
-        return pd.DataFrame(list(self._get_folds_as_json()))
+        return pd.DataFrame([row.copy() for row in self._get_folds_as_json()])
 
     def download_picke(self, path: str = None) -> str:
         results = list(self.get_folds())
         matrix = [[[] for x in range(9)] for i in range(10)]
         for result in results:
             test = int(result.name.replace("fold_", "").split("_")[0])
             sort = int(result.name.replace("fold_", "").split("_")[1])
```

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/resources/image.py` & `dorothy-sdk-1.4.8/dorothy_sdk/resources/image.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/resources/quality_annotation.py` & `dorothy-sdk-1.4.8/dorothy_sdk/resources/quality_annotation.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk/session.py` & `dorothy-sdk-1.4.8/dorothy_sdk/session.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk.egg-info/PKG-INFO` & `dorothy-sdk-1.4.8/dorothy_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorothy-sdk
-Version: 1.4.7
+Version: 1.4.8
 Summary: UNKNOWN
 Home-page: https://github.com/tb-brics/dorothy-sdk
 Author: Patrick Braz
 Author-email: patrickfbraz@poli.ufrj.br
 Maintainer: Patrick Braz
 Maintainer-email: patrickfbraz@poli.ufrj.br
 License: UNKNOWN
```

### Comparing `dorothy-sdk-1.4.7/dorothy_sdk.egg-info/SOURCES.txt` & `dorothy-sdk-1.4.8/dorothy_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.7/setup.py` & `dorothy-sdk-1.4.8/setup.py`

 * *Files identical despite different names*

