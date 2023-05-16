# Comparing `tmp/configstore-0.8.tar.gz` & `tmp/configstore-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configstore-0.8.tar", last modified: Thu May 19 20:07:37 2022, max compression
+gzip compressed data, was "configstore-0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `configstore-0.8.tar` & `configstore-0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      205 2021-11-03 17:20:56.147603 configstore-0.8/.github/dependabot.yml
--rw-r--r--   0        0        0     1750 2022-05-19 19:59:37.979291 configstore-0.8/.github/workflows/configstore.yml
--rw-r--r--   0        0        0      176 2021-11-03 17:21:09.387563 configstore-0.8/.gitignore
--rw-r--r--   0        0        0      733 2022-05-19 20:06:28.185788 configstore-0.8/CHANGELOG.rst
--rw-r--r--   0        0        0     1116 2021-11-03 17:20:56.147603 configstore-0.8/LICENSE
--rw-r--r--   0        0        0     2241 2021-11-03 01:20:46.154840 configstore-0.8/README.rst
--rw-r--r--   0        0        0      412 2022-05-19 20:06:28.185788 configstore-0.8/configstore/__init__.py
--rw-r--r--   0        0        0      304 2020-12-10 19:07:10.669556 configstore-0.8/configstore/backends/__init__.py
--rw-r--r--   0        0        0     1019 2021-11-03 17:20:56.147603 configstore-0.8/configstore/backends/awsssm.py
--rw-r--r--   0        0        0      441 2020-12-10 19:07:10.669556 configstore-0.8/configstore/backends/dict.py
--rw-r--r--   0        0        0      614 2021-11-03 17:20:56.147603 configstore-0.8/configstore/backends/docker_secret.py
--rw-r--r--   0        0        0      605 2021-11-03 17:20:56.147603 configstore-0.8/configstore/backends/dotenv.py
--rw-r--r--   0        0        0      273 2021-11-03 17:21:09.387563 configstore-0.8/configstore/backends/env_var.py
--rw-r--r--   0        0        0      934 2020-12-08 23:22:24.040601 configstore-0.8/configstore/converters.py
--rw-r--r--   0        0        0     2493 2022-05-19 19:49:52.619767 configstore-0.8/configstore/store.py
--rw-r--r--   0        0        0      999 2020-12-10 19:07:10.669556 configstore-0.8/example.py
--rw-r--r--   0        0        0     1094 2022-05-19 20:06:28.185788 configstore-0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2018-10-09 19:37:34.438005 configstore-0.8/tests/__init__.py
--rw-r--r--   0        0        0     3127 2018-10-09 19:13:31.042822 configstore-0.8/tests/test_awsssm.py
--rw-r--r--   0        0        0      667 2020-12-08 23:22:24.040601 configstore-0.8/tests/test_converters.py
--rw-r--r--   0        0        0      316 2020-12-10 19:07:10.669556 configstore-0.8/tests/test_dict.py
--rw-r--r--   0        0        0     1576 2018-10-09 19:13:39.726844 configstore-0.8/tests/test_docker_secret.py
--rw-r--r--   0        0        0     1280 2018-10-09 19:13:42.102851 configstore-0.8/tests/test_dotenv.py
--rw-r--r--   0        0        0      432 2018-10-09 19:13:44.318856 configstore-0.8/tests/test_env_var.py
--rw-r--r--   0        0        0     2275 2022-05-19 19:49:52.619767 configstore-0.8/tests/test_store.py
--rw-r--r--   0        0        0     4294 2022-05-19 19:49:52.619767 configstore-0.8/tests/test_z_integration.py
--rw-r--r--   0        0        0      938 2021-11-03 17:20:56.147603 configstore-0.8/tox.ini
--rw-r--r--   0        0        0     3319 1970-01-01 00:00:00.000000 configstore-0.8/PKG-INFO
+-rw-r--r--   0        0        0      205 2021-11-03 17:20:56.147603 configstore-0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     1669 2023-05-16 16:57:59.641238 configstore-0.9/.github/workflows/configstore.yml
+-rw-r--r--   0        0        0      195 2023-05-16 17:02:38.302458 configstore-0.9/.gitignore
+-rw-r--r--   0        0        0      857 2023-05-16 17:00:41.189951 configstore-0.9/CHANGELOG.rst
+-rw-r--r--   0        0        0     1097 2023-05-16 15:25:44.084892 configstore-0.9/LICENSE
+-rw-r--r--   0        0        0     2527 2023-05-16 16:57:59.641238 configstore-0.9/README.rst
+-rw-r--r--   0        0        0      412 2023-05-16 17:00:41.193951 configstore-0.9/configstore/__init__.py
+-rw-r--r--   0        0        0      304 2023-05-16 16:37:11.448075 configstore-0.9/configstore/backends/__init__.py
+-rw-r--r--   0        0        0     1019 2021-11-03 17:20:56.147603 configstore-0.9/configstore/backends/awsssm.py
+-rw-r--r--   0        0        0      441 2020-12-10 19:07:10.669556 configstore-0.9/configstore/backends/dict.py
+-rw-r--r--   0        0        0      614 2021-11-03 17:20:56.147603 configstore-0.9/configstore/backends/docker_secret.py
+-rw-r--r--   0        0        0      753 2023-05-16 16:57:59.641238 configstore-0.9/configstore/backends/dotenv.py
+-rw-r--r--   0        0        0      165 2023-05-16 17:02:38.294458 configstore-0.9/configstore/backends/env_var.py
+-rw-r--r--   0        0        0      934 2020-12-08 23:22:24.040601 configstore-0.9/configstore/converters.py
+-rw-r--r--   0        0        0     2493 2022-05-19 19:49:52.619767 configstore-0.9/configstore/store.py
+-rw-r--r--   0        0        0      999 2023-05-16 16:20:29.724194 configstore-0.9/example.py
+-rw-r--r--   0        0        0     1121 2023-05-16 16:57:59.641238 configstore-0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2018-10-09 19:37:34.438005 configstore-0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2018-10-09 19:13:31.042822 configstore-0.9/tests/test_awsssm.py
+-rw-r--r--   0        0        0      667 2020-12-08 23:22:24.040601 configstore-0.9/tests/test_converters.py
+-rw-r--r--   0        0        0      316 2020-12-10 19:07:10.669556 configstore-0.9/tests/test_dict.py
+-rw-r--r--   0        0        0     1576 2018-10-09 19:13:39.726844 configstore-0.9/tests/test_docker_secret.py
+-rw-r--r--   0        0        0     1280 2018-10-09 19:13:42.102851 configstore-0.9/tests/test_dotenv.py
+-rw-r--r--   0        0        0      432 2018-10-09 19:13:44.318856 configstore-0.9/tests/test_env_var.py
+-rw-r--r--   0        0        0     2275 2022-05-19 19:49:52.619767 configstore-0.9/tests/test_store.py
+-rw-r--r--   0        0        0     4294 2023-05-16 16:20:44.976251 configstore-0.9/tests/test_z_integration.py
+-rw-r--r--   0        0        0     1067 2023-05-16 16:57:59.641238 configstore-0.9/tox.ini
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 configstore-0.9/PKG-INFO
```

### Comparing `configstore-0.8/.github/workflows/configstore.yml` & `configstore-0.9/.github/workflows/configstore.yml`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,40 @@
 
 jobs:
 
   prepare:
     runs-on: ubuntu-latest
     steps:
       - name: Create matrix
-        uses: fabiocaccamo/create-matrix-action@v2
+        uses: fabiocaccamo/create-matrix-action@v3
         id: make_matrix
         with:
           matrix: |
-            python-version {3.10}, tox-env {py310,coverage,pkg}
-            python-version {3.9}, tox-env {py39}
-            python-version {3.8}, tox-env {py38}
-            python-version {3.7}, tox-env {py37}
+            python-version {3.11}, tox-env {py311,py311-pydotenv,coverage,pkg}
+            python-version {3.10}, tox-env {py310}
     outputs:
       matrix: ${{ steps.make_matrix.outputs.matrix }}
 
   test:
     runs-on: ubuntu-latest
     needs: prepare
     strategy:
       fail-fast: false
       matrix:
         include: ${{fromJson(needs.prepare.outputs.matrix)}}
 
     steps:
-      - uses: actions/checkout@v3.0.2
+      - uses: actions/checkout@v3.5.2
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3.1.2
+        uses: actions/setup-python@v4.6.0
         with:
           python-version: ${{ matrix.python-version }}
           cache: pip
           cache-dependency-path: 'pyproject.toml'
-      - uses: actions/cache@v3.0.2
+      - uses: actions/cache@v3.3.1
         with:
           path: |
             .tox
           key: configstore-${{ matrix.tox-env }}-v2-${{ hashFiles('pyproject.toml') }}
           restore-keys: configstore-${{ matrix.tox-env }}-v2-
       - name: Install dependencies
         run: |
@@ -52,11 +50,11 @@
   slack-workflow-status:
     runs-on: ubuntu-latest
     if: always()
     needs:
       - test
     steps:
       - name: Send Slack notification
-        uses: Gamesight/slack-workflow-status@v1.0.1
+        uses: Gamesight/slack-workflow-status@v1.2.0
         with:
           repo_token: ${{ secrets.GITHUB_TOKEN }}
           slack_webhook_url: ${{ secrets.SLACK_WEBHOOK_URL }}
```

### Comparing `configstore-0.8/CHANGELOG.rst` & `configstore-0.9/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
  changelog for configstore
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
+v0.9
+====
+
+Test with Python 3.10 and 3.11.
+Add support for python-dotenv in DotenvBackend for compat
+with docker-compose.
+
+
 v0.8
 ====
 
 Test with Python 3.9 and Python 3.10.
 Support interpolation with more than one variable.
```

### Comparing `configstore-0.8/LICENSE` & `configstore-0.9/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017, 2018, 2019, 2020, 2021 Caravan Web Worker Cooperative, Inc
+Copyright (c) 2017-2022 Caravan Web Worker Cooperative, Inc
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `configstore-0.8/README.rst` & `configstore-0.9/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -24,28 +24,33 @@
 settings that are not secrets.
 
 configstore.DotenvBackend lets you put settings in a key-value format file, using the
 `dotenv module`_, which is useful for local development.
 This backend requires an optional dependency, so use a requirement like ``configstore[dotenv]``
 to get everything installed.
 
+If you are using docker-compose, `another dotenv module`_ is already installed and
+does not provide the same interface; use a requirement like `configstore[pydotenv]`
+instead.  DotenvBackend is automatically compatible.
+
 configstore.DockerSecretBackend can read `Docker secrets`_.
 This is a secure storage with first-class support in the Docker runtime and related
 tooling.
 
 configstore.AwsSsmBackend connects to the Parameter Store service that
 is part of `AWS Systems Manager`_.  This backend requires optional
 dependencies (boto3), so use a requirement like ``configstore[awsssm]``
 to get everything installed.
 
 Finally, configstore.DictBackend is useful to define a bunch of settings
 for testing or for defaults.
 
 .. _docker secrets: https://docs.docker.com/engine/swarm/secrets/
-.. _dotenv module: https://github.com/jpadilla/django-dotenv
+.. _dotenv module: https://pypi.org/project/django-dotenv/
+.. _another dotenv module: https://pypi.org/project/python-dotenv/
 .. _aws systems manager: https://docs.aws.amazon.com/systems-manager/latest/APIReference/Welcome.html
 
 
 Contributors
 ------------
 
 Original author: Antoine Reversat @crevetor
```

### Comparing `configstore-0.8/configstore/backends/awsssm.py` & `configstore-0.9/configstore/backends/awsssm.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/configstore/backends/docker_secret.py` & `configstore-0.9/configstore/backends/docker_secret.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/configstore/converters.py` & `configstore-0.9/configstore/converters.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/configstore/store.py` & `configstore-0.9/configstore/store.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/example.py` & `configstore-0.9/example.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/pyproject.toml` & `configstore-0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 requires = ["flit_core ~= 3.4.0"]
 build-backend = "flit_core.buildapi"
 
-[tool.flit.metadata]
-module = "configstore"
-author = "Caravan Coop"
-author-email = "hi@caravan.coop"
-home-page = "https://github.com/caravancoop/configstore"
-description-file = "README.rst"
+[project]
+dynamic = ["version", "description"]
+name = "configstore"
+authors = [ { name = "Caravan Coop", email = "hi@caravan.coop" } ]
+readme = "README.rst"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
     "Topic :: System :: Installation/Setup",
     "Topic :: System :: Systems Administration",
 ]
-requires = [
+requires-python = ">= 3"
+dependencies = [
 ]
 
-[tool.flit.metadata.requires-extra]
+[project.optional-dependencies]
 # Note that django-dotenv does not actually use or need Django
 dotenv = ["django-dotenv"]
+# Alternate dotenv module, used by docker-compose
+pydotenv = ["python-dotenv"]
 awsssm = ["boto3"]
 
-[tool.flit.metadata.urls]
-Documentation = "https://github.com/caravancoop/configstore/blob/main/example.py"
+[project.urls]
+Homepage = "https://github.com/caravancoop/configstore"
 Changelog = "https://github.com/caravancoop/configstore/blob/main/CHANGELOG.rst"
+Documentation = "https://github.com/caravancoop/configstore/blob/main/example.py"
```

### Comparing `configstore-0.8/tests/test_awsssm.py` & `configstore-0.9/tests/test_awsssm.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/tests/test_converters.py` & `configstore-0.9/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/tests/test_docker_secret.py` & `configstore-0.9/tests/test_docker_secret.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/tests/test_dotenv.py` & `configstore-0.9/tests/test_dotenv.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/tests/test_store.py` & `configstore-0.9/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/tests/test_z_integration.py` & `configstore-0.9/tests/test_z_integration.py`

 * *Files identical despite different names*

### Comparing `configstore-0.8/tox.ini` & `configstore-0.9/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 [tox]
-envlist = py39
+envlist = py311,py311-pydotenv
 # enable pyproject.toml support
-minversion = 3.4.0
+minversion = 4.5.1
 isolated_build = True
 
 [testenv]
 deps =
     flake8
     pretend
-    pytest >= 3.9
+    pytest >= 7.3.1
 extras =
     dotenv
     awsssm
 commands =
     flake8 configstore
     pytest {posargs}
 
+[testenv:py311-pydotenv]
+extras =
+    pydotenv
+    awsssm
+
 # TODO run tests against the installed sdist, not the source dir
 
 [testenv:coverage]
 deps =
     {[testenv]deps}
     coverage
 commands =
     coverage run -m pytest -qq {posargs}
     coverage report
 
 [testenv:pkg]
 deps =
-    flit == 3.4.*
-    pip == 21.3.*
-    twine
-    safety == 1.10.*
+    flit == 3.9.*
+    pip == 23.1.*
+    twine == 4.0.*
+    pip-audit == 2.5.*
+extras =
+    dotenv
+    pydotenv
+    awsssm
 commands =
     flit build
     twine check dist/*
-    safety check
+    pip-audit
 
 
 [flake8]
 max-line-length = 89
 exclude = .git,.tox,__pycache__,dist
 ignore = E731,N806
 show-source = True
```

### Comparing `configstore-0.8/PKG-INFO` & `configstore-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: configstore
-Version: 0.8
+Version: 0.9
 Summary: Retrieve settings and secrets from different storages.
-Home-page: https://github.com/caravancoop/configstore
-Author: Caravan Coop
-Author-email: hi@caravan.coop
+Author-email: Caravan Coop <hi@caravan.coop>
+Requires-Python: >= 3
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Requires-Dist: boto3 ; extra == "awsssm"
 Requires-Dist: django-dotenv ; extra == "dotenv"
+Requires-Dist: python-dotenv ; extra == "pydotenv"
 Project-URL: Changelog, https://github.com/caravancoop/configstore/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://github.com/caravancoop/configstore/blob/main/example.py
+Project-URL: Homepage, https://github.com/caravancoop/configstore
 Provides-Extra: awsssm
 Provides-Extra: dotenv
+Provides-Extra: pydotenv
 
 ~~~~~~~~~~~~~
  configstore
 ~~~~~~~~~~~~~
 
 configstore is a small pluggable library that lets you retrieve settings
 or secrets from a variety of storage systems to configure your app.
@@ -49,28 +49,33 @@
 settings that are not secrets.
 
 configstore.DotenvBackend lets you put settings in a key-value format file, using the
 `dotenv module`_, which is useful for local development.
 This backend requires an optional dependency, so use a requirement like ``configstore[dotenv]``
 to get everything installed.
 
+If you are using docker-compose, `another dotenv module`_ is already installed and
+does not provide the same interface; use a requirement like `configstore[pydotenv]`
+instead.  DotenvBackend is automatically compatible.
+
 configstore.DockerSecretBackend can read `Docker secrets`_.
 This is a secure storage with first-class support in the Docker runtime and related
 tooling.
 
 configstore.AwsSsmBackend connects to the Parameter Store service that
 is part of `AWS Systems Manager`_.  This backend requires optional
 dependencies (boto3), so use a requirement like ``configstore[awsssm]``
 to get everything installed.
 
 Finally, configstore.DictBackend is useful to define a bunch of settings
 for testing or for defaults.
 
 .. _docker secrets: https://docs.docker.com/engine/swarm/secrets/
-.. _dotenv module: https://github.com/jpadilla/django-dotenv
+.. _dotenv module: https://pypi.org/project/django-dotenv/
+.. _another dotenv module: https://pypi.org/project/python-dotenv/
 .. _aws systems manager: https://docs.aws.amazon.com/systems-manager/latest/APIReference/Welcome.html
 
 
 Contributors
 ------------
 
 Original author: Antoine Reversat @crevetor
```

