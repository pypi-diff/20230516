# Comparing `tmp/poetry_git_version_plugin-1.0.0.tar.gz` & `tmp/poetry_git_version_plugin-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-1.0.0.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-1.0.0a1.tar", max compression
```

## Comparing `poetry_git_version_plugin-1.0.0.tar` & `poetry_git_version_plugin-1.0.0a1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1056 2023-05-01 10:00:45.334318 poetry_git_version_plugin-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2023-05-01 19:09:05.377623 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      330 2023-05-01 17:55:14.202116 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     1551 2023-05-01 17:55:14.202116 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      837 2023-05-01 19:02:48.091434 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1114 2023-05-01 19:02:48.091434 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5882 2023-05-01 19:02:48.095434 poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0     2776 2023-05-01 19:08:44.061725 poetry_git_version_plugin-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4406 2023-05-01 19:02:48.095434 poetry_git_version_plugin-1.0.0/readme.md
--rw-r--r--   0        0        0     5958 1970-01-01 00:00:00.000000 poetry_git_version_plugin-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-16 16:01:30.779815 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     2264 2023-05-16 16:01:30.739815 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      837 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1114 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5882 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0      420 2023-05-16 16:01:30.739815 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/utils.py
+-rw-r--r--   0        0        0     2776 2023-05-10 13:06:49.087670 poetry_git_version_plugin-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4823 2023-05-16 16:01:30.739815 poetry_git_version_plugin-1.0.0a1/readme.md
+-rw-r--r--   0        0        0     6377 1970-01-01 00:00:00.000000 poetry_git_version_plugin-1.0.0a1/PKG-INFO
```

### Comparing `poetry_git_version_plugin-1.0.0/LICENSE` & `poetry_git_version_plugin-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0/pyproject.toml` & `poetry_git_version_plugin-1.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0/readme.md` & `poetry_git_version_plugin-1.0.0a1/readme.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,64 +34,80 @@
 [tool.poetry.dependencies]
 python = ">=3.8"
 poetry = ">=1.2.2"
 ```
 
 ## Configs
 
-
-### make_alpha_version
+### MAKE ALPHA VERSION
 
 If the tag is not found on the HEAD, then the version is built based on the last found tag and the HEAD.
 
 - type: bool
 - Default = true
-- Example: 1.3.2a5
+- Result: 1.3.2a5
 
 ```toml
+# Environment
+export PACKAGE_VERSION_MAKE_ALPHA_VERSION=true
+# pyproject.toml
 [tool.poetry-git-version-plugin]
 make_alpha_version = true
 ```
 
-### alpha_version_format
+### ALPHA VERSION FORMAT
 
 Format for alpha version
 
 - Type: str
 - Default = `'{version}a{distance}'`
 - Example:
   - alpha_version_format = '{version}a{distance}' -> `1.3.2a5`
   - alpha_version_format = '{version}a{distance}+{commit_hash}' -> `1.3.2a5+5babef6`
 - Available variables:
   - **version**: Last found tag
   - **distance**: Distance from last found tag to HEAD
   - **commit_hash**: Commit hash
 
 ```toml
+# Environment
+export PACKAGE_VERSION_ALPHA_VERSION_FORMAT='{version}a{distance}'
+# pyproject.toml
 [tool.poetry-git-version-plugin]
 alpha_version_format = '{version}a{distance}'
 ```
 
 ### Ignore errors
 
 Three variables to **ignore errors**
 
 - Type: bool
 - Default = true
 
 ```toml
-[tool.poetry-git-version-plugin]
 # Ignore mismatch error PEP 440 version format
+## Environment
+export PACKAGE_VERSION_IGNORE_PEP440=true
+## pyproject.toml
+[tool.poetry-git-version-plugin]
 ignore_pep440 = true
 
 # Ignore mismatch error PEP 440 public version format
+## Environment
+export PACKAGE_VERSION_IGNORE_PUBLIC_PEP440=true
+## pyproject.toml
+[tool.poetry-git-version-plugin]
 ignore_public_pep440 = true
 
 # Ignore all errors
 # including version not found errors
+## Environment
+export PACKAGE_VERSION_IGNORE_ERRORS=true
+## pyproject.toml
+[tool.poetry-git-version-plugin]
 ignore_errors = true
 ```
 
 ## Use cases
 
 ### Publishing python package to pypi via poetry with version equal to git tag
 
@@ -114,30 +130,24 @@
 ```
 
 - When creating a git tag: new package with version == {TAG}
 - When pushing to CI_DEFAULT_BRANCH: new package with version == {TAG}a{N}
 
 ### Publishing python package to private pypi via poetry with version equal to git tag and commit hash
 
-Change the alpha version template:
-
-```toml
-[tool.poetry-git-version-plugin]
-alpha_version_format = '{version}a{distance}+{commit_hash}'
-```
-
 .gitlab-ci.yml:
 
 ```yaml
 pypi:
   stage: publishing
   image: python:3.10
   tags:
     - docker
   script:
+    - export PACKAGE_VERSION_ALPHA_VERSION_FORMAT='{version}a{distance}+{commit_hash}'
     - poetry self add poetry-git-version-plugin
     - poetry config repositories.gitlab "https://gitlab.com/api/v4/projects/$CI_PROJECT_ID/packages/pypi"
     - poetry config http-basic.gitlab gitlab-ci-token "$CI_JOB_TOKEN"
     - poetry publish -r gitlab --build
   rules:
     - if: $CI_COMMIT_TAG
     - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
```

### Comparing `poetry_git_version_plugin-1.0.0/PKG-INFO` & `poetry_git_version_plugin-1.0.0a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 1.0.0
+Version: 1.0.0a1
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -68,64 +68,80 @@
 [tool.poetry.dependencies]
 python = ">=3.8"
 poetry = ">=1.2.2"
 ```
 
 ## Configs
 
-
-### make_alpha_version
+### MAKE ALPHA VERSION
 
 If the tag is not found on the HEAD, then the version is built based on the last found tag and the HEAD.
 
 - type: bool
 - Default = true
-- Example: 1.3.2a5
+- Result: 1.3.2a5
 
 ```toml
+# Environment
+export PACKAGE_VERSION_MAKE_ALPHA_VERSION=true
+# pyproject.toml
 [tool.poetry-git-version-plugin]
 make_alpha_version = true
 ```
 
-### alpha_version_format
+### ALPHA VERSION FORMAT
 
 Format for alpha version
 
 - Type: str
 - Default = `'{version}a{distance}'`
 - Example:
   - alpha_version_format = '{version}a{distance}' -> `1.3.2a5`
   - alpha_version_format = '{version}a{distance}+{commit_hash}' -> `1.3.2a5+5babef6`
 - Available variables:
   - **version**: Last found tag
   - **distance**: Distance from last found tag to HEAD
   - **commit_hash**: Commit hash
 
 ```toml
+# Environment
+export PACKAGE_VERSION_ALPHA_VERSION_FORMAT='{version}a{distance}'
+# pyproject.toml
 [tool.poetry-git-version-plugin]
 alpha_version_format = '{version}a{distance}'
 ```
 
 ### Ignore errors
 
 Three variables to **ignore errors**
 
 - Type: bool
 - Default = true
 
 ```toml
-[tool.poetry-git-version-plugin]
 # Ignore mismatch error PEP 440 version format
+## Environment
+export PACKAGE_VERSION_IGNORE_PEP440=true
+## pyproject.toml
+[tool.poetry-git-version-plugin]
 ignore_pep440 = true
 
 # Ignore mismatch error PEP 440 public version format
+## Environment
+export PACKAGE_VERSION_IGNORE_PUBLIC_PEP440=true
+## pyproject.toml
+[tool.poetry-git-version-plugin]
 ignore_public_pep440 = true
 
 # Ignore all errors
 # including version not found errors
+## Environment
+export PACKAGE_VERSION_IGNORE_ERRORS=true
+## pyproject.toml
+[tool.poetry-git-version-plugin]
 ignore_errors = true
 ```
 
 ## Use cases
 
 ### Publishing python package to pypi via poetry with version equal to git tag
 
@@ -148,30 +164,24 @@
 ```
 
 - When creating a git tag: new package with version == {TAG}
 - When pushing to CI_DEFAULT_BRANCH: new package with version == {TAG}a{N}
 
 ### Publishing python package to private pypi via poetry with version equal to git tag and commit hash
 
-Change the alpha version template:
-
-```toml
-[tool.poetry-git-version-plugin]
-alpha_version_format = '{version}a{distance}+{commit_hash}'
-```
-
 .gitlab-ci.yml:
 
 ```yaml
 pypi:
   stage: publishing
   image: python:3.10
   tags:
     - docker
   script:
+    - export PACKAGE_VERSION_ALPHA_VERSION_FORMAT='{version}a{distance}+{commit_hash}'
     - poetry self add poetry-git-version-plugin
     - poetry config repositories.gitlab "https://gitlab.com/api/v4/projects/$CI_PROJECT_ID/packages/pypi"
     - poetry config http-basic.gitlab gitlab-ci-token "$CI_JOB_TOKEN"
     - poetry publish -r gitlab --build
   rules:
     - if: $CI_COMMIT_TAG
     - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
```

