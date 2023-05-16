# Comparing `tmp/hyp3_sdk-2.0.2.tar.gz` & `tmp/hyp3_sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyp3_sdk-2.0.2.tar", last modified: Fri May  5 19:13:18 2023, max compression
+gzip compressed data, was "hyp3_sdk-2.1.0.tar", last modified: Tue May 16 18:36:33 2023, max compression
```

## Comparing `hyp3_sdk-2.0.2.tar` & `hyp3_sdk-2.1.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.378377 hyp3_sdk-2.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.378377 hyp3_sdk-2.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.382377 hyp3_sdk-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/distribute.yml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/labeled-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/notify-downstream.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/release-template-comment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/tag-version.yml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.gitleaks.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/.trufflehog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.382377 hyp3_sdk-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/docs/sdk_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.374376 hyp3_sdk-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.382377 hyp3_sdk-2.0.2/src/hyp3_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/hyp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/src/hyp3_sdk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.382377 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 19:13:18.000000 hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:18.386377 hyp3_sdk-2.0.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/data/product.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/test_hyp3.py
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-05 19:12:26.000000 hyp3_sdk-2.0.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.650898 hyp3_sdk-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.642897 hyp3_sdk-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/distribute.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/labeled-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/notify-downstream.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/release-template-comment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/tag-version.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.gitleaks.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.trufflehog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/docs/sdk_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/docs/search_other_user_jobs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:36:33.650898 hyp3_sdk-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.642897 hyp3_sdk-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/src/hyp3_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19133 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/data/product.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/test_hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/test_util.py
```

### Comparing `hyp3_sdk-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `hyp3_sdk-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/.github/workflows/distribute.yml` & `hyp3_sdk-2.1.0/.github/workflows/distribute.yml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/.github/workflows/notify-downstream.yml` & `hyp3_sdk-2.1.0/.github/workflows/notify-downstream.yml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/.gitignore` & `hyp3_sdk-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/.gitleaks.toml` & `hyp3_sdk-2.1.0/.gitleaks.toml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/CHANGELOG.md` & `hyp3_sdk-2.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [PEP 440](https://www.python.org/dev/peps/pep-0440/) 
 and uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.1.0]
+### Added
+* The `HyP3.find_jobs` method now includes a `user_id` parameter that allows retrieving jobs for a given user.
+  If not provided, jobs are retrieved for the current user.
 
 ## [2.0.2]
 ### Added
 * 20 m can now be provided to the `resolution` keyword argument of `hyp3.submit_rtc_job` and `hyp3.prepare_rtc_job`.
 
 ## [2.0.1]
 ### Fixed
```

### Comparing `hyp3_sdk-2.0.2/CODE_OF_CONDUCT.md` & `hyp3_sdk-2.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/LICENSE` & `hyp3_sdk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/PKG-INFO` & `hyp3_sdk-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyp3_sdk
-Version: 2.0.2
+Version: 2.1.0
 Summary: A python wrapper around the HyP3 API
 Author-email: ASF APD/Tools Team <uaf-asf-apd@alaska.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ASFHyP3/hyp3-sdk
 Project-URL: Bug Tracker, https://github.com/ASFHyP3/hyp3-sdk/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hyp3_sdk-2.0.2/README.md` & `hyp3_sdk-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/docs/sdk_example.ipynb` & `hyp3_sdk-2.1.0/docs/sdk_example.ipynb`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/pyproject.toml` & `hyp3_sdk-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/src/hyp3_sdk/exceptions.py` & `hyp3_sdk-2.1.0/src/hyp3_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/src/hyp3_sdk/hyp3.py` & `hyp3_sdk-2.1.0/src/hyp3_sdk/hyp3.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 from hyp3_sdk.jobs import Batch, Job
 
 PROD_API = 'https://hyp3-api.asf.alaska.edu'
 TEST_API = 'https://hyp3-test-api.asf.alaska.edu'
 
 
 class HyP3:
-    """A python wrapper around the HyP3 API"""
+    """A python wrapper around the HyP3 API.
+
+    Warning: All jobs submitted to HyP3 are publicly visible. For more information, see
+    https://hyp3-docs.asf.alaska.edu/#public-visibility-of-jobs
+    """
 
     def __init__(self, api_url: str = PROD_API, username: Optional[str] = None, password: Optional[str] = None,
                  prompt: bool = False):
         """If username and password are not provided, attempts to use credentials from a `.netrc` file.
 
         Args:
             api_url: Address of the HyP3 API
@@ -38,31 +42,36 @@
             username = input('NASA Earthdata Login username: ')
         if password is None and prompt:
             password = getpass('NASA Earthdata Login password: ')
 
         self.session = hyp3_sdk.util.get_authenticated_session(username, password)
         self.session.headers.update({'User-Agent': f'{hyp3_sdk.__name__}/{hyp3_sdk.__version__}'})
 
-    def find_jobs(self, start: Optional[datetime] = None, end: Optional[datetime] = None,
-                  status_code: Optional[str] = None, name: Optional[str] = None,
+    def find_jobs(self,
+                  user_id: Optional[str] = None,
+                  start: Optional[datetime] = None,
+                  end: Optional[datetime] = None,
+                  status_code: Optional[str] = None,
+                  name: Optional[str] = None,
                   job_type: Optional[str] = None) -> Batch:
         """Gets a Batch of jobs from HyP3 matching the provided search criteria
 
         Args:
+            user_id: only jobs submitted by this user (defaults to the current user)
             start: only jobs submitted after given time
             end: only jobs submitted before given time
             status_code: only jobs matching this status (SUCCEEDED, FAILED, RUNNING, PENDING)
             name: only jobs with this name
             job_type: only jobs with this job_type
 
         Returns:
             A Batch object containing the found jobs
         """
         params = {}
-        for param_name in ('start', 'end', 'status_code', 'name', 'job_type'):
+        for param_name in ('user_id', 'start', 'end', 'status_code', 'name', 'job_type'):
             param_value = locals().get(param_name)
             if param_value is not None:
                 if isinstance(param_value, datetime):
                     if param_value.tzinfo is None:
                         param_value = param_value.replace(tzinfo=timezone.utc)
                     param_value = param_value.isoformat(timespec='seconds')
```

### Comparing `hyp3_sdk-2.0.2/src/hyp3_sdk/jobs.py` & `hyp3_sdk-2.1.0/src/hyp3_sdk/jobs.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/src/hyp3_sdk/util.py` & `hyp3_sdk-2.1.0/src/hyp3_sdk/util.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/PKG-INFO` & `hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyp3-sdk
-Version: 2.0.2
+Version: 2.1.0
 Summary: A python wrapper around the HyP3 API
 Author-email: ASF APD/Tools Team <uaf-asf-apd@alaska.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ASFHyP3/hyp3-sdk
 Project-URL: Bug Tracker, https://github.com/ASFHyP3/hyp3-sdk/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hyp3_sdk-2.0.2/src/hyp3_sdk.egg-info/SOURCES.txt` & `hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 .github/workflows/notify-downstream.yml
 .github/workflows/release-template-comment.yml
 .github/workflows/release.yml
 .github/workflows/static-analysis.yml
 .github/workflows/tag-version.yml
 .github/workflows/test.yml
 docs/sdk_example.ipynb
+docs/search_other_user_jobs.ipynb
 src/hyp3_sdk/__init__.py
 src/hyp3_sdk/exceptions.py
 src/hyp3_sdk/hyp3.py
 src/hyp3_sdk/jobs.py
 src/hyp3_sdk/util.py
 src/hyp3_sdk.egg-info/PKG-INFO
 src/hyp3_sdk.egg-info/SOURCES.txt
```

### Comparing `hyp3_sdk-2.0.2/tests/conftest.py` & `hyp3_sdk-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/tests/data/product.zip` & `hyp3_sdk-2.1.0/tests/data/product.zip`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/tests/test_exceptions.py` & `hyp3_sdk-2.1.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/tests/test_hyp3.py` & `hyp3_sdk-2.1.0/tests/test_hyp3.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,32 @@
     batch = api.find_jobs()
     assert len(batch) == 3
     assert 'next' not in responses.calls[0].request.params
     assert 'next' in responses.calls[1].request.params
 
 
 @responses.activate
+def test_find_jobs_user_id(get_mock_job):
+    with patch('hyp3_sdk.util.get_authenticated_session', mock_get_authenticated_session):
+        api = HyP3()
+
+    responses.add(responses.GET, urljoin(api.url, '/jobs?user_id=foo'),
+                  json={'jobs': []}, match_querystring=True)
+
+    responses.add(responses.GET, urljoin(api.url, '/jobs?user_id=bar'),
+                  json={'jobs': [get_mock_job(name='job1').to_dict()]}, match_querystring=True)
+
+    batch = api.find_jobs(user_id='foo')
+    assert len(batch) == 0
+
+    batch = api.find_jobs(user_id='bar')
+    assert len(batch) == 1
+
+
+@responses.activate
 def test_find_jobs_start():
     with patch('hyp3_sdk.util.get_authenticated_session', mock_get_authenticated_session):
         api = HyP3()
 
     responses.add(responses.GET, urljoin(api.url, '/jobs?start=2021-01-01T00%3A00%3A00%2B00%3A00'),
                   json={'jobs': []}, match_querystring=True)
```

### Comparing `hyp3_sdk-2.0.2/tests/test_jobs.py` & `hyp3_sdk-2.1.0/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.0.2/tests/test_util.py` & `hyp3_sdk-2.1.0/tests/test_util.py`

 * *Files identical despite different names*

