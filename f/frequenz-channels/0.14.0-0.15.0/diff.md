# Comparing `tmp/frequenz-channels-0.14.0.tar.gz` & `tmp/frequenz-channels-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-channels-0.14.0.tar", last modified: Wed Mar 29 10:57:16 2023, max compression
+gzip compressed data, was "frequenz-channels-0.15.0.tar", last modified: Tue May 16 09:51:44 2023, max compression
```

## Comparing `frequenz-channels-0.14.0.tar` & `frequenz-channels-0.15.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:16.108621 frequenz-channels-0.14.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-03-29 10:57:16.108621 frequenz-channels-0.14.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:16.100621 frequenz-channels-0.14.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:16.100621 frequenz-channels-0.14.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/docs/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/docs/mkdocstrings_autoapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:16.104621 frequenz-channels-0.14.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (122)     2589 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-29 10:57:16.108621 frequenz-channels-0.14.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:16.096621 frequenz-channels-0.14.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:16.096621 frequenz-channels-0.14.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:16.104621 frequenz-channels-0.14.0/src/frequenz/channels/
--rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6819 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/_anycast.py
--rw-r--r--   0 runner    (1001) docker     (122)     6348 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/_bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (122)    12090 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:16.108621 frequenz-channels-0.14.0/src/frequenz/channels/util/
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3671 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/util/_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     3942 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/util/_merge.py
--rw-r--r--   0 runner    (1001) docker     (122)     3625 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/util/_merge_named.py
--rw-r--r--   0 runner    (1001) docker     (122)     6617 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/util/_select.py
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-03-29 10:57:04.000000 frequenz-channels-0.14.0/src/frequenz/channels/util/_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 10:57:16.108621 frequenz-channels-0.14.0/src/frequenz_channels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-03-29 10:57:16.000000 frequenz-channels-0.14.0/src/frequenz_channels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-03-29 10:57:16.000000 frequenz-channels-0.14.0/src/frequenz_channels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-29 10:57:16.000000 frequenz-channels-0.14.0/src/frequenz_channels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-03-29 10:57:16.000000 frequenz-channels-0.14.0/src/frequenz_channels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-29 10:57:16.000000 frequenz-channels-0.14.0/src/frequenz_channels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.800384 frequenz-channels-0.15.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-16 09:51:44.800384 frequenz-channels-0.15.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2589 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 09:51:44.800384 frequenz-channels-0.15.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.792384 frequenz-channels-0.15.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/src/frequenz/channels/
+-rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7095 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_anycast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6348 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12090 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.796384 frequenz-channels-0.15.0/src/frequenz/channels/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4259 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_merge_named.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6686 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_select.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24885 2023-05-16 09:51:32.000000 frequenz-channels-0.15.0/src/frequenz/channels/util/_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 09:51:44.800384 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 09:51:44.000000 frequenz-channels-0.15.0/src/frequenz_channels.egg-info/top_level.txt
```

### Comparing `frequenz-channels-0.14.0/CONTRIBUTING.md` & `frequenz-channels-0.15.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/LICENSE` & `frequenz-channels-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/PKG-INFO` & `frequenz-channels-0.15.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-channels
-Version: 0.14.0
+Version: 0.15.0
 Summary: Channel implementations for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-channels-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-channels-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-channels-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-channels-python/discussions/categories/support
```

### Comparing `frequenz-channels-0.14.0/README.md` & `frequenz-channels-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/docs/css/mkdocstrings.css` & `frequenz-channels-0.15.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/docs/css/style.css` & `frequenz-channels-0.15.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/docs/logo.png` & `frequenz-channels-0.15.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/docs/mkdocstrings_autoapi.py` & `frequenz-channels-0.15.0/docs/mkdocstrings_autoapi.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/mkdocs.yml` & `frequenz-channels-0.15.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/pyproject.toml` & `frequenz-channels-0.15.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 [build-system]
 requires = [
-    "setuptools >= 65.3.0, < 66",
-    "setuptools_scm[toml] >= 7.0.5, < 8",
-    "wheel"
+  "setuptools >= 65.3.0, < 66",
+  "setuptools_scm[toml] >= 7.0.5, < 8",
+  "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "frequenz-channels"
 description = "Channel implementations for Python"
 readme = "README.md"
 license = { text = "MIT" }
-keywords = [ "frequenz", "channel" ]
+keywords = ["frequenz", "channel"]
 classifiers = [
-   "Development Status :: 3 - Alpha",
-   "Intended Audience :: Developers",
-   "License :: OSI Approved :: MIT License",
-   "Programming Language :: Python :: 3",
-   "Programming Language :: Python :: 3 :: Only",
-   "Programming Language :: Python :: 3.8",
-   "Programming Language :: Python :: 3.9",
-   "Programming Language :: Python :: 3.10",
-   "Topic :: Software Development :: Libraries",
+  "Development Status :: 3 - Alpha",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">= 3.8, < 4"
-dependencies = [
-    "watchfiles >= 0.15.0",
-]
-dynamic = [ "version" ]
+dependencies = ["watchfiles >= 0.15.0"]
+dynamic = ["version"]
 
 [[project.authors]]
-name ="Frequenz Energy-as-a-Service GmbH"
+name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
 docs = [
-    "mike >= 1.1.2, < 2",
-    "mkdocs-gen-files >= 0.4.0, < 0.5.0",
-    "mkdocs-literate-nav >= 0.4.0, < 0.5.0",
-    "mkdocs-material >= 8.5.7, < 9",
-    "mkdocs-section-index >= 0.3.4, < 0.4.0",
-    "mkdocstrings[python] >= 0.19.0, < 0.20.0",
+  "mike >= 1.1.2, < 2",
+  "mkdocs-gen-files >= 0.4.0, < 0.5.0",
+  "mkdocs-literate-nav >= 0.4.0, < 0.5.0",
+  "mkdocs-material >= 8.5.7, < 9",
+  "mkdocs-section-index >= 0.3.4, < 0.4.0",
+  "mkdocstrings[python] >= 0.19.0, < 0.20.0",
 ]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-channels-python/releases"
 Repository = "https://github.com/frequenz-floss/frequenz-channels-python"
 Issues = "https://github.com/frequenz-floss/frequenz-channels-python/issues"
 Support = "https://github.com/frequenz-floss/frequenz-channels-python/discussions/categories/support"
@@ -53,26 +51,33 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 
 [tool.pylint.similarities]
-ignore-comments=['yes']
-ignore-docstrings=['yes']
-ignore-imports=['no']
-min-similarity-lines=40
+ignore-comments = ['yes']
+ignore-docstrings = ['yes']
+ignore-imports = ['no']
+min-similarity-lines = 40
 
 [tool.pylint.messages_control]
 # disable wrong-import-order, ungrouped-imports because it conflicts with isort
 disable = ["too-few-public-methods", "wrong-import-order", "ungrouped-imports"]
 [tool.pylint.'DESIGN']
-max-attributes=12
+max-attributes = 12
 
 [tool.isort]
 profile = "black"
 line_length = 88
 src_paths = ["src", "examples", "tests"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
-required_plugins = [ "pytest-asyncio", "pytest-mock" ]
+required_plugins = ["pytest-asyncio", "pytest-mock"]
+markers = [
+  "integration: integration tests (deselect with '-m \"not integration\"')",
+]
+
+[[tool.mypy.overrides]]
+module = ["async_solipsism", "async_solipsism.*"]
+ignore_missing_imports = true
```

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/__init__.py` & `frequenz-channels-0.15.0/src/frequenz/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/_anycast.py` & `frequenz-channels-0.15.0/src/frequenz/channels/_anycast.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """A channel for sending data across async tasks."""
 
 from __future__ import annotations
 
 from asyncio import Condition
 from collections import deque
-from typing import Deque, Generic, Optional
+from typing import Deque, Generic, Type
 
 from ._base_classes import Receiver as BaseReceiver
 from ._base_classes import Sender as BaseSender
 from ._base_classes import T
 from ._exceptions import ChannelClosedError, ReceiverStoppedError, SenderError
 
 
@@ -147,43 +147,47 @@
             async with self._chan.send_cv:
                 await self._chan.send_cv.wait()
         self._chan.deque.append(msg)
         async with self._chan.recv_cv:
             self._chan.recv_cv.notify(1)
 
 
+class _Empty:
+    """A sentinel value to indicate that a value has not been set."""
+
+
 class Receiver(BaseReceiver[T]):
     """A receiver to receive messages from an Anycast channel.
 
     Should not be created directly, but through the `Anycast.new_receiver()`
     method.
     """
 
     def __init__(self, chan: Anycast[T]) -> None:
         """Create a channel receiver.
 
         Args:
             chan: A reference to the channel that this receiver belongs to.
         """
         self._chan = chan
-        self._next: Optional[T] = None
+        self._next: T | Type[_Empty] = _Empty
 
     async def ready(self) -> bool:
         """Wait until the receiver is ready with a value or an error.
 
         Once a call to `ready()` has finished, the value should be read with
         a call to `consume()` (`receive()` or iterated over). The receiver will
         remain ready (this method will return immediately) until it is
         consumed.
 
         Returns:
             Whether the receiver is still active.
         """
         # if a message is already ready, then return immediately.
-        if self._next is not None:
+        if self._next is not _Empty:
             return True
 
         while len(self._chan.deque) == 0:
             if self._chan.closed:
                 return False
             async with self._chan.recv_cv:
                 await self._chan.recv_cv.wait()
@@ -198,16 +202,19 @@
         Returns:
             The next value that was received.
 
         Raises:
             ReceiverStoppedError: if the receiver stopped producing messages.
             ReceiverError: if there is some problem with the receiver.
         """
-        if self._next is None and self._chan.closed:
+        if self._next is _Empty and self._chan.closed:
             raise ReceiverStoppedError(self) from ChannelClosedError(self._chan)
 
         assert (
-            self._next is not None
+            self._next is not _Empty
         ), "`consume()` must be preceeded by a call to `ready()`"
-        next_val = self._next
-        self._next = None
+        # mypy doesn't understand that the assert above ensures that self._next is not
+        # _Sentinel.  So we have to use a type ignore here.
+        next_val: T = self._next  # type: ignore[assignment]
+        self._next = _Empty
+
         return next_val
```

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/_base_classes.py` & `frequenz-channels-0.15.0/src/frequenz/channels/_base_classes.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/_bidirectional.py` & `frequenz-channels-0.15.0/src/frequenz/channels/_bidirectional.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/_broadcast.py` & `frequenz-channels-0.15.0/src/frequenz/channels/_broadcast.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/_exceptions.py` & `frequenz-channels-0.15.0/src/frequenz/channels/_exceptions.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/util/__init__.py` & `frequenz-channels-0.15.0/src/frequenz/channels/util/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,29 +13,38 @@
   multiple receivers into a single stream.
 
 * [MergeNamed][frequenz.channels.util.MergeNamed]:
   A [receiver][frequenz.channels.Receiver] that merge messages coming from
   multiple receivers into a single named stream, allowing to identify the
   origin of each message.
 
+* [Timer][frequenz.channels.util.Timer]:
+  A [receiver][frequenz.channels.Receiver] that ticks at certain intervals.
+
 * [Select][frequenz.channels.util.Select]: A helper to select the next
   available message for each [receiver][frequenz.channels.Receiver] in a group
   of receivers.
-
-* [Timer][frequenz.channels.util.Timer]:
-  A [receiver][frequenz.channels.Receiver] that emits a *now* `timestamp`
-  every `interval` seconds.
 """
 
 from ._file_watcher import FileWatcher
 from ._merge import Merge
 from ._merge_named import MergeNamed
 from ._select import Select
-from ._timer import Timer
+from ._timer import (
+    MissedTickPolicy,
+    SkipMissedAndDrift,
+    SkipMissedAndResync,
+    Timer,
+    TriggerAllMissed,
+)
 
 __all__ = [
     "FileWatcher",
     "Merge",
     "MergeNamed",
-    "Select",
+    "MissedTickPolicy",
     "Timer",
+    "Select",
+    "SkipMissedAndDrift",
+    "SkipMissedAndResync",
+    "TriggerAllMissed",
 ]
```

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/util/_file_watcher.py` & `frequenz-channels-0.15.0/src/frequenz/channels/util/_file_watcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """A Channel receiver for watching for new (or modified) files."""
+
+from __future__ import annotations
+
 import asyncio
 import pathlib
+from dataclasses import dataclass
 from enum import Enum
-from typing import List, Optional, Set, Union
 
 from watchfiles import Change, awatch
 from watchfiles.main import FileChange
 
 from .._base_classes import Receiver
 from .._exceptions import ReceiverStoppedError
 
 
-class FileWatcher(Receiver[pathlib.Path]):
+class FileWatcher(Receiver["FileWatcher.Event"]):
     """A channel receiver that watches for file events."""
 
     class EventType(Enum):
         """Available types of changes to watch for."""
 
         CREATE = Change.added
         MODIFY = Change.modified
         DELETE = Change.deleted
 
+    @dataclass(frozen=True)
+    class Event:
+        """A file change event."""
+
+        type: FileWatcher.EventType
+        """The type of change that was observed."""
+        path: pathlib.Path
+        """The path where the change was observed."""
+
     def __init__(
         self,
-        paths: List[Union[pathlib.Path, str]],
-        event_types: Optional[Set[EventType]] = None,
+        paths: list[pathlib.Path | str],
+        event_types: set[EventType] | None = None,
     ) -> None:
         """Create a `FileWatcher` instance.
 
         Args:
             paths: Paths to watch for changes.
             event_types: Types of events to watch for or `None` to watch for
                 all event types.
@@ -42,23 +54,34 @@
         self.event_types = event_types
         self._stop_event = asyncio.Event()
         self._paths = [
             path if isinstance(path, pathlib.Path) else pathlib.Path(path)
             for path in paths
         ]
         self._awatch = awatch(
-            *self._paths,
-            stop_event=self._stop_event,
-            watch_filter=lambda change, path_str: (
-                change in [event_type.value for event_type in event_types]  # type: ignore
-                and pathlib.Path(path_str).is_file()
-            ),
+            *self._paths, stop_event=self._stop_event, watch_filter=self._filter_events
         )
-        self._awatch_stopped_exc: Optional[Exception] = None
-        self._changes: Set[FileChange] = set()
+        self._awatch_stopped_exc: Exception | None = None
+        self._changes: set[FileChange] = set()
+
+    def _filter_events(
+        self,
+        change: Change,
+        path: str,  # pylint: disable=unused-argument
+    ) -> bool:
+        """Filter events based on the event type and path.
+
+        Args:
+            change: The type of change to be notified.
+            path: The path of the file that changed.
+
+        Returns:
+            Whether the event should be notified.
+        """
+        return change in [event_type.value for event_type in self.event_types]
 
     def __del__(self) -> None:
         """Cleanup registered watches.
 
         `awatch` passes the `stop_event` to a separate task/thread. This way
         `awatch` getting destroyed properly. The background task will continue
         until the signal is received.
@@ -87,25 +110,25 @@
         try:
             self._changes = await self._awatch.__anext__()
         except StopAsyncIteration as err:
             self._awatch_stopped_exc = err
 
         return True
 
-    def consume(self) -> pathlib.Path:
-        """Return the latest change once `ready` is complete.
+    def consume(self) -> Event:
+        """Return the latest event once `ready` is complete.
 
         Returns:
-            The next change that was received.
+            The next event that was received.
 
         Raises:
             ReceiverStoppedError: if there is some problem with the receiver.
         """
         if not self._changes and self._awatch_stopped_exc is not None:
             raise ReceiverStoppedError(self) from self._awatch_stopped_exc
 
         assert self._changes, "`consume()` must be preceeded by a call to `ready()`"
-        change = self._changes.pop()
         # Tuple of (Change, path) returned by watchfiles
-        _, path_str = change
-        path = pathlib.Path(path_str)
-        return path
+        change, path_str = self._changes.pop()
+        return FileWatcher.Event(
+            type=FileWatcher.EventType(change), path=pathlib.Path(path_str)
+        )
```

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/util/_merge.py` & `frequenz-channels-0.15.0/src/frequenz/channels/util/_merge.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,16 @@
             for name, recv in self._receivers.items()
         }
         self._results: Deque[T] = deque(maxlen=len(self._receivers))
 
     def __del__(self) -> None:
         """Cleanup any pending tasks."""
         for task in self._pending:
-            task.cancel()
+            if not task.done() and task.get_loop().is_running():
+                task.cancel()
 
     async def stop(self) -> None:
         """Stop the `Merge` instance and cleanup any pending tasks."""
         for task in self._pending:
             task.cancel()
         await asyncio.gather(*self._pending, return_exceptions=True)
         self._pending = set()
```

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/util/_merge_named.py` & `frequenz-channels-0.15.0/src/frequenz/channels/util/_merge_named.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
             for name, recv in self._receivers.items()
         }
         self._results: Deque[Tuple[str, T]] = deque(maxlen=len(self._receivers))
 
     def __del__(self) -> None:
         """Cleanup any pending tasks."""
         for task in self._pending:
-            task.cancel()
+            if not task.done() and task.get_loop().is_running():
+                task.cancel()
 
     async def stop(self) -> None:
         """Stop the `MergeNamed` instance and cleanup any pending tasks."""
         for task in self._pending:
             task.cancel()
         await asyncio.gather(*self._pending, return_exceptions=True)
         self._pending = set()
```

### Comparing `frequenz-channels-0.14.0/src/frequenz/channels/util/_select.py` & `frequenz-channels-0.15.0/src/frequenz/channels/util/_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,16 @@
         self._result: Dict[str, Optional[_ReadyReceiver]] = {
             name: None for name in self._receivers
         }
 
     def __del__(self) -> None:
         """Cleanup any pending tasks."""
         for task in self._pending:
-            task.cancel()
+            if not task.done() and task.get_loop().is_running():
+                task.cancel()
 
     async def stop(self) -> None:
         """Stop the `Select` instance and cleanup any pending tasks."""
         for task in self._pending:
             task.cancel()
         await asyncio.gather(*self._pending, return_exceptions=True)
         self._pending = set()
```

### Comparing `frequenz-channels-0.14.0/src/frequenz_channels.egg-info/PKG-INFO` & `frequenz-channels-0.15.0/src/frequenz_channels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-channels
-Version: 0.14.0
+Version: 0.15.0
 Summary: Channel implementations for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-channels-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-channels-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-channels-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-channels-python/discussions/categories/support
```

### Comparing `frequenz-channels-0.14.0/src/frequenz_channels.egg-info/SOURCES.txt` & `frequenz-channels-0.15.0/src/frequenz_channels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

