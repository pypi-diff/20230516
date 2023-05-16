# Comparing `tmp/poetry_git_version_plugin-1.0.0a1.tar.gz` & `tmp/poetry_git_version_plugin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_git_version_plugin-1.0.0a1.tar", max compression
+gzip compressed data, was "poetry_git_version_plugin-1.0.1.tar", max compression
```

## Comparing `poetry_git_version_plugin-1.0.0a1.tar` & `poetry_git_version_plugin-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1056 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/LICENSE
--rw-r--r--   0        0        0        0 2023-05-16 16:01:30.779815 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/__init__.py
--rw-r--r--   0        0        0      330 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/commands.py
--rw-r--r--   0        0        0     2264 2023-05-16 16:01:30.739815 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/config.py
--rw-r--r--   0        0        0      837 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/exceptions.py
--rw-r--r--   0        0        0     1114 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/plugins.py
--rw-r--r--   0        0        0     5882 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/services.py
--rw-r--r--   0        0        0      420 2023-05-16 16:01:30.739815 poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/utils.py
--rw-r--r--   0        0        0     2776 2023-05-10 13:06:49.087670 poetry_git_version_plugin-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4823 2023-05-16 16:01:30.739815 poetry_git_version_plugin-1.0.0a1/readme.md
--rw-r--r--   0        0        0     6377 1970-01-01 00:00:00.000000 poetry_git_version_plugin-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-16 16:05:39.606634 poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/commands.py
+-rw-r--r--   0        0        0     2264 2023-05-16 16:01:30.739815 poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/config.py
+-rw-r--r--   0        0        0      837 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/exceptions.py
+-rw-r--r--   0        0        0     1114 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/plugins.py
+-rw-r--r--   0        0        0     5882 2023-05-10 13:06:49.083670 poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/services.py
+-rw-r--r--   0        0        0      420 2023-05-16 16:01:30.739815 poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/utils.py
+-rw-r--r--   0        0        0     2776 2023-05-10 13:06:49.087670 poetry_git_version_plugin-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4823 2023-05-16 16:01:30.739815 poetry_git_version_plugin-1.0.1/readme.md
+-rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 poetry_git_version_plugin-1.0.1/PKG-INFO
```

### Comparing `poetry_git_version_plugin-1.0.0a1/LICENSE` & `poetry_git_version_plugin-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/config.py` & `poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/config.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/exceptions.py` & `poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/plugins.py` & `poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0a1/poetry_git_version_plugin/services.py` & `poetry_git_version_plugin-1.0.1/poetry_git_version_plugin/services.py`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0a1/pyproject.toml` & `poetry_git_version_plugin-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0a1/readme.md` & `poetry_git_version_plugin-1.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `poetry_git_version_plugin-1.0.0a1/PKG-INFO` & `poetry_git_version_plugin-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-git-version-plugin
-Version: 1.0.0a1
+Version: 1.0.1
 Summary: Poetry plugin to get package version from git
 Home-page: https://gitlab.com/rocshers/python/poetry-git-version-plugin
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

