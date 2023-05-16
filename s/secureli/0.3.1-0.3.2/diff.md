# Comparing `tmp/secureli-0.3.1.tar.gz` & `tmp/secureli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.3.1.tar", max compression
+gzip compressed data, was "secureli-0.3.2.tar", max compression
```

## Comparing `secureli-0.3.1.tar` & `secureli-0.3.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11343 2023-05-15 18:34:33.762111 secureli-0.3.1/LICENSE
--rw-r--r--   0        0        0    10572 2023-05-15 18:34:33.766111 secureli-0.3.1/README.md
--rw-r--r--   0        0        0     1825 2023-05-15 18:34:33.766111 secureli-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0    30307 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/actions/__init__.py
--rw-r--r--   0        0        0    10747 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10013 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/actions/scan.py
--rw-r--r--   0        0        0      787 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/actions/update.py
--rw-r--r--   0        0        0     6165 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/main.py
--rw-r--r--   0        0        0        0 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     1752 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/files/build.txt
--rw-r--r--   0        0        0     1271 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      478 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      619 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      409 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0      642 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0     2211 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/services/language_support.py
--rw-r--r--   0        0        0     4090 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3074 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0     1372 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-05-15 18:34:33.766111 secureli-0.3.1/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0    11413 1970-01-01 00:00:00.000000 secureli-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-16 19:41:50.019156 secureli-0.3.2/LICENSE
+-rw-r--r--   0        0        0    10572 2023-05-16 19:41:50.019156 secureli-0.3.2/README.md
+-rw-r--r--   0        0        0     1825 2023-05-16 19:41:50.019156 secureli-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 19:41:50.019156 secureli-0.3.2/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 19:41:50.019156 secureli-0.3.2/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-05-16 19:41:50.019156 secureli-0.3.2/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-05-16 19:41:50.019156 secureli-0.3.2/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0    30307 2023-05-16 19:41:50.019156 secureli-0.3.2/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-05-16 19:41:50.019156 secureli-0.3.2/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    10747 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10013 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/actions/update.py
+-rw-r--r--   0        0        0     6165 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     1752 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/__init__.py
+-rw-r--r--   0        0        0     4883 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0     1271 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      619 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0     1151 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      409 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      433 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0      642 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0     2211 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4090 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3074 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0     1372 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-05-16 19:41:50.027157 secureli-0.3.2/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0    11413 1970-01-01 00:00:00.000000 secureli-0.3.2/PKG-INFO
```

### Comparing `secureli-0.3.1/LICENSE` & `secureli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/README.md` & `secureli-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/pyproject.toml` & `secureli-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.3.1"
+version = "0.3.2"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
```

### Comparing `secureli-0.3.1/secureli/abstractions/echo.py` & `secureli-0.3.2/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/abstractions/lexer_guesser.py` & `secureli-0.3.2/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/abstractions/pre_commit.py` & `secureli-0.3.2/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/actions/action.py` & `secureli-0.3.2/secureli/actions/action.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/actions/build.py` & `secureli-0.3.2/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/actions/initializer.py` & `secureli-0.3.2/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/actions/scan.py` & `secureli-0.3.2/secureli/actions/scan.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/actions/setup.py` & `secureli-0.3.2/secureli/actions/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from secureli.services.language_support import supported_languages
 
 
 class SetupAction:
     """Arranges various properties needed to set up the application itself."""
 
-    repo_url = "https://bitbucket.org/slalom-consulting/secureli"
-    confluence_url = "https://slalom.atlassian.net/wiki/spaces/STFT"
+    repo_url = "https://github.com/slalombuild/secureli/blob/main/CONTRIBUTING.md"
+    docs_url = "https://github.com/slalombuild/secureli/wiki"
 
     def __init__(self, epilog_template_data: str):
         self.epilog_template_data = epilog_template_data
 
     def create_epilog(self):
         """Renders the epilog to display as part of the application help text."""
         template = jinja2.Template(source=self.epilog_template_data)
         return template.render(
             supported_languages=supported_languages,
-            confluence_url=self.confluence_url,
+            confluence_url=self.docs_url,
             repo_url=self.repo_url,
         )
```

### Comparing `secureli-0.3.1/secureli/actions/update.py` & `secureli-0.3.2/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/container.py` & `secureli-0.3.2/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/main.py` & `secureli-0.3.2/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/repositories/repo_files.py` & `secureli-0.3.2/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/repositories/secureli_config.py` & `secureli-0.3.2/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/repositories/settings.py` & `secureli-0.3.2/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/resources/files/build.txt` & `secureli-0.3.2/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.3.2/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/resources/files/java-pre-commit.yaml` & `secureli-0.3.2/secureli/resources/files/java-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/resources/files/python-pre-commit.yaml` & `secureli-0.3.2/secureli/resources/files/python-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.3.2/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/resources/read_resource.py` & `secureli-0.3.2/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/resources/slugify.py` & `secureli-0.3.2/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/services/git_ignore.py` & `secureli-0.3.2/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/services/language_analyzer.py` & `secureli-0.3.2/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/services/language_support.py` & `secureli-0.3.2/secureli/services/language_support.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/services/logging.py` & `secureli-0.3.2/secureli/services/logging.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/services/scanner.py` & `secureli-0.3.2/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/services/secureli_ignore.py` & `secureli-0.3.2/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/services/updater.py` & `secureli-0.3.2/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/settings.py` & `secureli-0.3.2/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/utilities/git_meta.py` & `secureli-0.3.2/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/secureli/utilities/patterns.py` & `secureli-0.3.2/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.3.1/PKG-INFO` & `secureli-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.3.1
+Version: 0.3.2
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

