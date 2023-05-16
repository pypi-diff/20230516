# Comparing `tmp/autohooks_plugin_flake8-23.4.0.tar.gz` & `tmp/autohooks_plugin_flake8-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autohooks_plugin_flake8-23.4.0.tar", max compression
+gzip compressed data, was "autohooks_plugin_flake8-23.5.0.tar", max compression
```

## Comparing `autohooks_plugin_flake8-23.4.0.tar` & `autohooks_plugin_flake8-23.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/LICENSE
--rw-r--r--   0        0        0     2614 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/README.md
--rw-r--r--   0        0        0      806 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/autohooks/plugins/flake8/__init__.py
--rw-r--r--   0        0        0      103 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/autohooks/plugins/flake8/__version__.py
--rw-r--r--   0        0        0     3752 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/autohooks/plugins/flake8/flake8.py
--rw-r--r--   0        0        0     2038 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/pyproject.toml
--rw-r--r--   0        0        0      721 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/tests/flake8_test.py
--rw-r--r--   0        0        0      112 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/tests/pyproject.test.toml
--rw-r--r--   0        0        0     4231 2023-04-20 08:10:28.528077 autohooks_plugin_flake8-23.4.0/tests/test_flake8.py
--rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 autohooks_plugin_flake8-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-16 07:23:56.776212 autohooks_plugin_flake8-23.5.0/LICENSE
+-rw-r--r--   0        0        0     2614 2023-05-16 07:23:56.776212 autohooks_plugin_flake8-23.5.0/README.md
+-rw-r--r--   0        0        0      806 2023-05-16 07:23:56.776212 autohooks_plugin_flake8-23.5.0/autohooks/plugins/flake8/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-16 07:23:56.776212 autohooks_plugin_flake8-23.5.0/autohooks/plugins/flake8/__version__.py
+-rw-r--r--   0        0        0     3752 2023-05-16 07:23:56.776212 autohooks_plugin_flake8-23.5.0/autohooks/plugins/flake8/flake8.py
+-rw-r--r--   0        0        0     2040 2023-05-16 07:23:56.776212 autohooks_plugin_flake8-23.5.0/pyproject.toml
+-rw-r--r--   0        0        0      721 2023-05-16 07:23:56.776212 autohooks_plugin_flake8-23.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-16 07:23:56.776212 autohooks_plugin_flake8-23.5.0/tests/flake8_test.py
+-rw-r--r--   0        0        0      112 2023-05-16 07:23:56.780212 autohooks_plugin_flake8-23.5.0/tests/pyproject.test.toml
+-rw-r--r--   0        0        0     4231 2023-05-16 07:23:56.780212 autohooks_plugin_flake8-23.5.0/tests/test_flake8.py
+-rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 autohooks_plugin_flake8-23.5.0/PKG-INFO
```

### Comparing `autohooks_plugin_flake8-23.4.0/LICENSE` & `autohooks_plugin_flake8-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_flake8-23.4.0/README.md` & `autohooks_plugin_flake8-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_flake8-23.4.0/autohooks/plugins/flake8/__init__.py` & `autohooks_plugin_flake8-23.5.0/autohooks/plugins/flake8/__init__.py`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_flake8-23.4.0/autohooks/plugins/flake8/flake8.py` & `autohooks_plugin_flake8-23.5.0/autohooks/plugins/flake8/flake8.py`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_flake8-23.4.0/pyproject.toml` & `autohooks_plugin_flake8-23.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autohooks-plugin-flake8"
-version = "23.4.0"
+version = "23.5.0"
 readme = "README.md"
 description = "An autohooks plugin for python code linting via flake8."
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 packages = [
   { include = "autohooks" },
   { include = "tests", format = "sdist" },
@@ -32,23 +32,23 @@
   "linting",
   "hooks",
   "flake8",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
-flake8 = "5.0.4"
+flake8 = ">=5.0.4"
 autohooks = ">=21.3.0"
 
 [tool.poetry.dev-dependencies]
 mypy = ">=0.981"
 pontos = ">=22.7.2"
 autohooks-plugin-black = ">=22.7.0"
 autohooks-plugin-isort = ">=22.3.0"
-coverage = "^7.2.3"
+coverage = "^7.2.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
```

### Comparing `autohooks_plugin_flake8-23.4.0/tests/__init__.py` & `autohooks_plugin_flake8-23.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_flake8-23.4.0/tests/flake8_test.py` & `autohooks_plugin_flake8-23.5.0/tests/flake8_test.py`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_flake8-23.4.0/tests/test_flake8.py` & `autohooks_plugin_flake8-23.5.0/tests/test_flake8.py`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_flake8-23.4.0/PKG-INFO` & `autohooks_plugin_flake8-23.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autohooks-plugin-flake8
-Version: 23.4.0
+Version: 23.5.0
 Summary: An autohooks plugin for python code linting via flake8.
 Home-page: https://github.com/greenbone/autohooks-plugin-flake8
 License: GPL-3.0-or-later
 Keywords: git,linting,hooks,flake8
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.7.2,<4.0.0
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Dist: autohooks (>=21.3.0)
-Requires-Dist: flake8 (==5.0.4)
+Requires-Dist: flake8 (>=5.0.4)
 Project-URL: Repository, https://github.com/greenbone/autohooks-plugin-flake8
 Description-Content-Type: text/markdown
 
 ![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
 # autohooks-plugin-flake8
```

