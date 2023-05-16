# Comparing `tmp/exasol-script-languages-container-ci-1.0.0.tar.gz` & `tmp/exasol_script_languages_container_ci-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol-script-languages-container-ci-1.0.0.tar", max compression
+gzip compressed data, was "exasol_script_languages_container_ci-1.1.0.tar", max compression
```

## Comparing `exasol-script-languages-container-ci-1.0.0.tar` & `exasol_script_languages_container_ci-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/LICENSE
--rw-r--r--   0        0        0       95 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/cli/__init__.py
--rw-r--r--   0        0        0       50 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/cli/cli.py
--rw-r--r--   0        0        0        0 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/cli/commands/__init__.py
--rw-r--r--   0        0        0     1658 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/cli/commands/run_ci.py
--rw-r--r--   0        0        0     2566 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/cli/commands/run_release.py
--rw-r--r--   0        0        0        0 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/__init__.py
--rw-r--r--   0        0        0     1304 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/asset_uploader.py
--rw-r--r--   0        0        0     1677 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/branch_config.py
--rw-r--r--   0        0        0     4992 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci.py
--rw-r--r--   0        0        0     2595 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_build.py
--rw-r--r--   0        0        0      806 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_export.py
--rw-r--r--   0        0        0      978 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_push.py
--rw-r--r--   0        0        0     1104 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_security_scan.py
--rw-r--r--   0        0        0     1693 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_test.py
--rw-r--r--   0        0        0     1150 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/common.py
--rw-r--r--   0        0        0     1501 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/git_access.py
--rw-r--r--   0        0        0     1223 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py
--rw-r--r--   0        0        0     2786 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/release.py
--rw-r--r--   0        0        0     2443 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/release_uploader.py
--rwxr-xr-x   0        0        0      125 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/main.py
--rw-r--r--   0        0        0      784 2023-03-28 12:01:27.694136 exasol-script-languages-container-ci-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 exasol-script-languages-container-ci-1.0.0/setup.py
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 exasol-script-languages-container-ci-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-16 07:14:42.008871 exasol_script_languages_container_ci-1.1.0/LICENSE
+-rw-r--r--   0        0        0       95 2023-05-16 07:14:42.008871 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 07:14:42.008871 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/cli/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-16 07:14:42.008871 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-05-16 07:14:42.008871 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-16 07:14:42.008871 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/cli/commands/run_ci.py
+-rw-r--r--   0        0        0     2566 2023-05-16 07:14:42.008871 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/cli/commands/run_release.py
+-rw-r--r--   0        0        0        0 2023-05-16 07:14:42.008871 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/__init__.py
+-rw-r--r--   0        0        0     1304 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/asset_uploader.py
+-rw-r--r--   0        0        0     1677 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/branch_config.py
+-rw-r--r--   0        0        0     4992 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci.py
+-rw-r--r--   0        0        0     2595 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_build.py
+-rw-r--r--   0        0        0      806 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_export.py
+-rw-r--r--   0        0        0      978 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_push.py
+-rw-r--r--   0        0        0     1104 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_security_scan.py
+-rw-r--r--   0        0        0     1693 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_test.py
+-rw-r--r--   0        0        0     1150 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/common.py
+-rw-r--r--   0        0        0     1501 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/git_access.py
+-rw-r--r--   0        0        0     1223 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py
+-rw-r--r--   0        0        0     2786 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/release.py
+-rw-r--r--   0        0        0     2443 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/release_uploader.py
+-rwxr-xr-x   0        0        0      125 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/main.py
+-rw-r--r--   0        0        0      785 2023-05-16 07:14:42.012872 exasol_script_languages_container_ci-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci-1.1.0/PKG-INFO
```

### Comparing `exasol-script-languages-container-ci-1.0.0/LICENSE` & `exasol_script_languages_container_ci-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/cli/commands/run_ci.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/cli/commands/run_ci.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/cli/commands/run_release.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/cli/commands/run_release.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/asset_uploader.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/asset_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/branch_config.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/branch_config.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_build.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_build.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_export.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_export.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_push.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_push.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_security_scan.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/ci_test.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/ci_test.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/common.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/common.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/git_access.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/git_access.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/release.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/release.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/exasol_script_languages_container_ci/lib/release_uploader.py` & `exasol_script_languages_container_ci-1.1.0/exasol_script_languages_container_ci/lib/release_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol-script-languages-container-ci-1.0.0/pyproject.toml` & `exasol_script_languages_container_ci-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "exasol-script-languages-container-ci"
-version = "1.0.0"
+version = "1.1.0"
 description = "Implements CI builds for script-language-container."
 
 license = "MIT"
 
 authors = [
     "Thomas Uebensee <ext.thomas.uebensee@exasol.com>"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4.0"
 click = "^8.0.3"
 GitPython = ">=3.1.0"
-exasol-script-languages-container-tool = "0.16.0"
+exasol-script-languages-container-tool = "^0.17.0"
 exasol-integration-test-docker-environment = "^1.4.0"
 PyGithub = "^1.55.0"
 setuptools = "^67.6.0"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

