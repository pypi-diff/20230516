# Comparing `tmp/ml2p-0.3.4.tar.gz` & `tmp/ml2p-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml2p-0.3.4.tar", last modified: Fri Feb 24 10:06:38 2023, max compression
+gzip compressed data, was "ml2p-0.3.5.tar", last modified: Tue May 16 08:53:48 2023, max compression
```

## Comparing `ml2p-0.3.4.tar` & `ml2p-0.3.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:06:38.378112 ml2p-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-24 10:06:26.000000 ml2p-0.3.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-02-24 10:06:26.000000 ml2p-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-24 10:06:26.000000 ml2p-0.3.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-02-24 10:06:26.000000 ml2p-0.3.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-24 10:06:26.000000 ml2p-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-24 10:06:26.000000 ml2p-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-02-24 10:06:38.378112 ml2p-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-02-24 10:06:26.000000 ml2p-0.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:06:38.374112 ml2p-0.3.4/ml2p/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:06:38.378112 ml2p-0.3.4/ml2p/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli_commands/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli_commands/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli_commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli_commands/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli_commands/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli_commands/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli_commands/training_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/cli_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-02-24 10:06:26.000000 ml2p-0.3.4/ml2p/hyperparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:06:38.374112 ml2p-0.3.4/ml2p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-02-24 10:06:38.000000 ml2p-0.3.4/ml2p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-02-24 10:06:38.000000 ml2p-0.3.4/ml2p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 10:06:38.000000 ml2p-0.3.4/ml2p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-24 10:06:38.000000 ml2p-0.3.4/ml2p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-24 10:06:38.000000 ml2p-0.3.4/ml2p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 10:06:38.000000 ml2p-0.3.4/ml2p.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-24 10:06:26.000000 ml2p-0.3.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-24 10:06:26.000000 ml2p-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-24 10:06:38.378112 ml2p-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-24 10:06:26.000000 ml2p-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:06:38.378112 ml2p-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:06:38.378112 ml2p-0.3.4/tests/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/cli_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/cli_commands/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/cli_commands/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/cli_commands/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/cli_commands/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/cli_commands/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/cli_commands/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/cli_commands/test_training_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/cli_commands/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 10:06:38.378112 ml2p-0.3.4/tests/fixture_files/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/fixture_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-02-24 10:06:26.000000 ml2p-0.3.4/tests/test_hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-24 10:06:26.000000 ml2p-0.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.998045 ml2p-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 08:53:36.000000 ml2p-0.3.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-16 08:53:36.000000 ml2p-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 08:53:36.000000 ml2p-0.3.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-16 08:53:36.000000 ml2p-0.3.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-16 08:53:36.000000 ml2p-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 08:53:36.000000 ml2p-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-16 08:53:47.998045 ml2p-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-16 08:53:36.000000 ml2p-0.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.994045 ml2p-0.3.5/ml2p/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.994045 ml2p-0.3.5/ml2p/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli_commands/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli_commands/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli_commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli_commands/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli_commands/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli_commands/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli_commands/training_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/cli_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-16 08:53:36.000000 ml2p-0.3.5/ml2p/hyperparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.994045 ml2p-0.3.5/ml2p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-16 08:53:47.000000 ml2p-0.3.5/ml2p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-16 08:53:47.000000 ml2p-0.3.5/ml2p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:53:47.000000 ml2p-0.3.5/ml2p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-16 08:53:47.000000 ml2p-0.3.5/ml2p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 08:53:47.000000 ml2p-0.3.5/ml2p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 08:53:47.000000 ml2p-0.3.5/ml2p.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 08:53:36.000000 ml2p-0.3.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 08:53:36.000000 ml2p-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-16 08:53:47.998045 ml2p-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 08:53:36.000000 ml2p-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.994045 ml2p-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.998045 ml2p-0.3.5/tests/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/cli_commands/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/cli_commands/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/cli_commands/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/cli_commands/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/cli_commands/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/cli_commands/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/cli_commands/test_training_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/cli_commands/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.998045 ml2p-0.3.5/tests/fixture_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/fixture_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-16 08:53:36.000000 ml2p-0.3.5/tests/test_hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-16 08:53:36.000000 ml2p-0.3.5/tox.ini
```

### Comparing `ml2p-0.3.4/.gitignore` & `ml2p-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/HISTORY.rst` & `ml2p-0.3.5/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 History
 =======
 
+0.3.5 (2023-05-16)
+------------------
+
+* Pin Flask version.
+
 0.3.4 (2023-02-24)
 ------------------
 
 * Ensure that logging is passed to SageMaker logs.
 
 0.3.3 (2023-02-17)
 ------------------
```

### Comparing `ml2p-0.3.4/LICENSE` & `ml2p-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/PKG-INFO` & `ml2p-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml2p
-Version: 0.3.4
+Version: 0.3.5
 Summary: A minimum-lovable machine-learning pipeline, built on top of AWS SageMaker.
 Home-page: http://github.com/prodigyfinance/ml2p
 Author: Prodigy Finance
 Author-email: devops@prodigyfinance.com
 License: ISCL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `ml2p-0.3.4/README.rst` & `ml2p-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/cli.py` & `ml2p-0.3.5/ml2p/cli.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/cli_commands/dataset.py` & `ml2p-0.3.5/ml2p/cli_commands/dataset.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/cli_commands/endpoint.py` & `ml2p-0.3.5/ml2p/cli_commands/endpoint.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/cli_commands/init.py` & `ml2p-0.3.5/ml2p/cli_commands/init.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/cli_commands/model.py` & `ml2p-0.3.5/ml2p/cli_commands/model.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/cli_commands/notebook.py` & `ml2p-0.3.5/ml2p/cli_commands/notebook.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/cli_commands/repo.py` & `ml2p-0.3.5/ml2p/cli_commands/repo.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/cli_commands/training_job.py` & `ml2p-0.3.5/ml2p/cli_commands/training_job.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/cli_commands/utils.py` & `ml2p-0.3.5/ml2p/cli_commands/utils.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/core.py` & `ml2p-0.3.5/ml2p/core.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/docker.py` & `ml2p-0.3.5/ml2p/docker.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/errors.py` & `ml2p-0.3.5/ml2p/errors.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p/hyperparameters.py` & `ml2p-0.3.5/ml2p/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/ml2p.egg-info/PKG-INFO` & `ml2p-0.3.5/ml2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml2p
-Version: 0.3.4
+Version: 0.3.5
 Summary: A minimum-lovable machine-learning pipeline, built on top of AWS SageMaker.
 Home-page: http://github.com/prodigyfinance/ml2p
 Author: Prodigy Finance
 Author-email: devops@prodigyfinance.com
 License: ISCL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `ml2p-0.3.4/ml2p.egg-info/SOURCES.txt` & `ml2p-0.3.5/ml2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/setup.cfg` & `ml2p-0.3.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.4
+current_version = 0.3.5
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `ml2p-0.3.4/setup.py` & `ml2p-0.3.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from setuptools import find_packages, setup
 
-requirements = ["boto3", "click", "Flask", "Flask-API", "PyYAML"]
+requirements = [
+    "boto3",
+    "click",
+    "Flask<2.3",
+    "Flask-API",
+    "PyYAML",
+]
 
 def_requirements = [
     "black",
     "bumpversion",
     "coverage",
     "flake8",
     "isort",
@@ -13,15 +19,15 @@
     "radon[flake8]",
     "tox",
     "moto",
 ]
 
 setup(
     name="ml2p",
-    version="0.3.4",
+    version="0.3.5",
     url="http://github.com/prodigyfinance/ml2p",
     license="ISCL",
     description=(
         "A minimum-lovable machine-learning pipeline, built on top of AWS SageMaker."
     ),
     long_description=open("README.rst", "r").read(),
     author="Prodigy Finance",
```

### Comparing `ml2p-0.3.4/tests/cli_commands/test_dataset.py` & `ml2p-0.3.5/tests/cli_commands/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/cli_commands/test_endpoint.py` & `ml2p-0.3.5/tests/cli_commands/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/cli_commands/test_init.py` & `ml2p-0.3.5/tests/cli_commands/test_init.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/cli_commands/test_model.py` & `ml2p-0.3.5/tests/cli_commands/test_model.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/cli_commands/test_notebook.py` & `ml2p-0.3.5/tests/cli_commands/test_notebook.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/cli_commands/test_repo.py` & `ml2p-0.3.5/tests/cli_commands/test_repo.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/cli_commands/test_training_job.py` & `ml2p-0.3.5/tests/cli_commands/test_training_job.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/cli_commands/test_utils.py` & `ml2p-0.3.5/tests/cli_commands/test_utils.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/fixtures.py` & `ml2p-0.3.5/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/test_cli.py` & `ml2p-0.3.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/test_core.py` & `ml2p-0.3.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/test_docker.py` & `ml2p-0.3.5/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/test_errors.py` & `ml2p-0.3.5/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ml2p-0.3.4/tests/test_hyperparameters.py` & `ml2p-0.3.5/tests/test_hyperparameters.py`

 * *Files identical despite different names*

