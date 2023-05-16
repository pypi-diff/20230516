# Comparing `tmp/hyp3_sdk-2.1.0.tar.gz` & `tmp/hyp3_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyp3_sdk-2.1.0.tar", last modified: Tue May 16 18:36:33 2023, max compression
+gzip compressed data, was "hyp3_sdk-2.1.1.tar", last modified: Tue May 16 20:03:41 2023, max compression
```

## Comparing `hyp3_sdk-2.1.0.tar` & `hyp3_sdk-2.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.650898 hyp3_sdk-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.642897 hyp3_sdk-2.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/distribute.yml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/labeled-pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/notify-downstream.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/release-template-comment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/tag-version.yml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.gitleaks.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/.trufflehog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/docs/sdk_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/docs/search_other_user_jobs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:36:33.650898 hyp3_sdk-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.642897 hyp3_sdk-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/src/hyp3_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19133 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/hyp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/src/hyp3_sdk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 18:36:33.000000 hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:36:33.646898 hyp3_sdk-2.1.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/data/product.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/test_hyp3.py
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-16 18:35:28.000000 hyp3_sdk-2.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.911531 hyp3_sdk-2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.907531 hyp3_sdk-2.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.907531 hyp3_sdk-2.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.907531 hyp3_sdk-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/workflows/distribute.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/workflows/labeled-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/workflows/notify-downstream.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/workflows/release-template-comment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/workflows/tag-version.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.gitleaks.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/.trufflehog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-16 20:03:41.911531 hyp3_sdk-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.907531 hyp3_sdk-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/docs/sdk_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/docs/search_other_user_jobs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:03:41.911531 hyp3_sdk-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.903531 hyp3_sdk-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.907531 hyp3_sdk-2.1.1/src/hyp3_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/src/hyp3_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/src/hyp3_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19133 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/src/hyp3_sdk/hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/src/hyp3_sdk/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/src/hyp3_sdk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.907531 hyp3_sdk-2.1.1/src/hyp3_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-16 20:03:41.000000 hyp3_sdk-2.1.1/src/hyp3_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-16 20:03:41.000000 hyp3_sdk-2.1.1/src/hyp3_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:03:41.000000 hyp3_sdk-2.1.1/src/hyp3_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:03:41.000000 hyp3_sdk-2.1.1/src/hyp3_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-16 20:03:41.000000 hyp3_sdk-2.1.1/src/hyp3_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 20:03:41.000000 hyp3_sdk-2.1.1/src/hyp3_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.907531 hyp3_sdk-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:03:41.907531 hyp3_sdk-2.1.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/tests/data/product.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/tests/test_hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-16 20:02:48.000000 hyp3_sdk-2.1.1/tests/test_util.py
```

### Comparing `hyp3_sdk-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `hyp3_sdk-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/.github/workflows/distribute.yml` & `hyp3_sdk-2.1.1/.github/workflows/distribute.yml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/.github/workflows/notify-downstream.yml` & `hyp3_sdk-2.1.1/.github/workflows/notify-downstream.yml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/.gitignore` & `hyp3_sdk-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/.gitleaks.toml` & `hyp3_sdk-2.1.1/.gitleaks.toml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/CHANGELOG.md` & `hyp3_sdk-2.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [PEP 440](https://www.python.org/dev/peps/pep-0440/) 
 and uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.1.1]
+### Fixed
+* The `user_id` parameter has been moved to the end of the `HyP3.find_jobs` parameter list, to avoid
+  introducing breaking changes for users who rely on the order of the parameters.
+
 ## [2.1.0]
 ### Added
 * The `HyP3.find_jobs` method now includes a `user_id` parameter that allows retrieving jobs for a given user.
   If not provided, jobs are retrieved for the current user.
 
 ## [2.0.2]
 ### Added
```

### Comparing `hyp3_sdk-2.1.0/CODE_OF_CONDUCT.md` & `hyp3_sdk-2.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/LICENSE` & `hyp3_sdk-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/PKG-INFO` & `hyp3_sdk-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyp3_sdk
-Version: 2.1.0
+Version: 2.1.1
 Summary: A python wrapper around the HyP3 API
 Author-email: ASF APD/Tools Team <uaf-asf-apd@alaska.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ASFHyP3/hyp3-sdk
 Project-URL: Bug Tracker, https://github.com/ASFHyP3/hyp3-sdk/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hyp3_sdk-2.1.0/README.md` & `hyp3_sdk-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/docs/sdk_example.ipynb` & `hyp3_sdk-2.1.1/docs/sdk_example.ipynb`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/docs/search_other_user_jobs.ipynb` & `hyp3_sdk-2.1.1/docs/search_other_user_jobs.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'cells'": "{0: {'source': '# Using the HyP3 SDK to search for jobs run by another user\\n\\nTo "*

 * *            'facilitate collaboration, HyP3 allows you to search for jobs run by other '*

 * *            'users.\\n\\nFollow [Using the HyP3 SDK for '*

 * *            'Python](https://nbviewer.jupyter.org/github/ASFHyP3/hyp3-sdk/blob/main/docs/sdk_example.ipynb) '*

 * *            'to install the `hyp3-sdk` package (version `2.1.1` or higher) and authenticate using '*

 * *            'your Earthdata credentials.\\n\\nSuppose yo […]*

```diff
@@ -1,13 +1,13 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
-            "source": "# Using the HyP3 SDK to search for jobs run by another user\n\nTo facilitate collaboration, HyP3 allows you to search for jobs run by other users.\n\nFollow [Using the HyP3 SDK for Python](https://nbviewer.jupyter.org/github/ASFHyP3/hyp3-sdk/blob/main/docs/sdk_example.ipynb) to install the `hyp3-sdk` package (version `2.1.0` or higher) and authenticate using your Earthdata credentials.\n\nSuppose you have run a number of RTC jobs with the name `rtc-example`. You can search for them using `find_jobs`:"
+            "source": "# Using the HyP3 SDK to search for jobs run by another user\n\nTo facilitate collaboration, HyP3 allows you to search for jobs run by other users.\n\nFollow [Using the HyP3 SDK for Python](https://nbviewer.jupyter.org/github/ASFHyP3/hyp3-sdk/blob/main/docs/sdk_example.ipynb) to install the `hyp3-sdk` package (version `2.1.1` or higher) and authenticate using your Earthdata credentials.\n\nSuppose you have run a number of RTC jobs with the name `rtc-example`. You can search for them using `find_jobs`:"
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": "from hyp3_sdk import HyP3\nhyp3 = HyP3()\nmy_rtc_jobs = hyp3.find_jobs(name='rtc-example')"
```

### Comparing `hyp3_sdk-2.1.0/pyproject.toml` & `hyp3_sdk-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/src/hyp3_sdk/exceptions.py` & `hyp3_sdk-2.1.1/src/hyp3_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/src/hyp3_sdk/hyp3.py` & `hyp3_sdk-2.1.1/src/hyp3_sdk/hyp3.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,35 +43,35 @@
         if password is None and prompt:
             password = getpass('NASA Earthdata Login password: ')
 
         self.session = hyp3_sdk.util.get_authenticated_session(username, password)
         self.session.headers.update({'User-Agent': f'{hyp3_sdk.__name__}/{hyp3_sdk.__version__}'})
 
     def find_jobs(self,
-                  user_id: Optional[str] = None,
                   start: Optional[datetime] = None,
                   end: Optional[datetime] = None,
                   status_code: Optional[str] = None,
                   name: Optional[str] = None,
-                  job_type: Optional[str] = None) -> Batch:
+                  job_type: Optional[str] = None,
+                  user_id: Optional[str] = None) -> Batch:
         """Gets a Batch of jobs from HyP3 matching the provided search criteria
 
         Args:
-            user_id: only jobs submitted by this user (defaults to the current user)
             start: only jobs submitted after given time
             end: only jobs submitted before given time
             status_code: only jobs matching this status (SUCCEEDED, FAILED, RUNNING, PENDING)
             name: only jobs with this name
             job_type: only jobs with this job_type
+            user_id: only jobs submitted by this user (defaults to the current user)
 
         Returns:
             A Batch object containing the found jobs
         """
         params = {}
-        for param_name in ('user_id', 'start', 'end', 'status_code', 'name', 'job_type'):
+        for param_name in ('start', 'end', 'status_code', 'name', 'job_type', 'user_id'):
             param_value = locals().get(param_name)
             if param_value is not None:
                 if isinstance(param_value, datetime):
                     if param_value.tzinfo is None:
                         param_value = param_value.replace(tzinfo=timezone.utc)
                     param_value = param_value.isoformat(timespec='seconds')
```

### Comparing `hyp3_sdk-2.1.0/src/hyp3_sdk/jobs.py` & `hyp3_sdk-2.1.1/src/hyp3_sdk/jobs.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/src/hyp3_sdk/util.py` & `hyp3_sdk-2.1.1/src/hyp3_sdk/util.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/PKG-INFO` & `hyp3_sdk-2.1.1/src/hyp3_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyp3-sdk
-Version: 2.1.0
+Version: 2.1.1
 Summary: A python wrapper around the HyP3 API
 Author-email: ASF APD/Tools Team <uaf-asf-apd@alaska.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ASFHyP3/hyp3-sdk
 Project-URL: Bug Tracker, https://github.com/ASFHyP3/hyp3-sdk/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hyp3_sdk-2.1.0/src/hyp3_sdk.egg-info/SOURCES.txt` & `hyp3_sdk-2.1.1/src/hyp3_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/tests/conftest.py` & `hyp3_sdk-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/tests/data/product.zip` & `hyp3_sdk-2.1.1/tests/data/product.zip`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/tests/test_exceptions.py` & `hyp3_sdk-2.1.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/tests/test_hyp3.py` & `hyp3_sdk-2.1.1/tests/test_hyp3.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/tests/test_jobs.py` & `hyp3_sdk-2.1.1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-2.1.0/tests/test_util.py` & `hyp3_sdk-2.1.1/tests/test_util.py`

 * *Files identical despite different names*

