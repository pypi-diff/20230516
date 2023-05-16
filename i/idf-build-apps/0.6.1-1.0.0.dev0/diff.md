# Comparing `tmp/idf-build-apps-0.6.1.tar.gz` & `tmp/idf_build_apps-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf-build-apps-0.6.1.tar", last modified: Wed May 10 02:23:31 2023, max compression
+gzip compressed data, was "idf_build_apps-1.0.0.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idf-build-apps-0.6.1.tar` & `idf_build_apps-1.0.0.dev0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      351 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.editorconfig
--rw-r--r--   0        0        0      123 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.gitattributes
--rw-r--r--   0        0        0      253 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3707 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.gitignore
--rw-r--r--   0        0        0     1077 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/.readthedocs.yml
--rw-r--r--   0        0        0     4125 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/CHANGELOG.md
--rw-r--r--   0        0        0     1834 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/LICENSE
--rw-r--r--   0        0        0     3843 2023-05-10 02:23:28.438667 idf-build-apps-0.6.1/README.md
--rw-r--r--   0        0        0       33 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/config_file.md
--rw-r--r--   0        0        0    10368 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/index.rst
--rw-r--r--   0        0        0     3651 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/docs/manifest.md
--rw-r--r--   0        0        0      481 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    22146 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/app.py
--rw-r--r--   0        0        0     2768 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/config.py
--rw-r--r--   0        0        0     2187 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6026 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/log.py
--rw-r--r--   0        0        0    31784 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6144 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     5695 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     6577 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/license_header.txt
--rw-r--r--   0        0        0     1874 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/tests/conftest.py
--rw-r--r--   0        0        0     2181 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/tests/test_build.py
--rw-r--r--   0        0        0    10242 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/tests/test_finder.py
--rw-r--r--   0        0        0      995 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/tests/test_manifest.py
--rw-r--r--   0        0        0     2394 2023-05-10 02:23:28.442667 idf-build-apps-0.6.1/tests/test_utils.py
--rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 idf-build-apps-0.6.1/setup.py
--rw-r--r--   0        0        0     5495 1970-01-01 00:00:00.000000 idf-build-apps-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.editorconfig
+-rw-r--r--   0        0        0      123 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.gitattributes
+-rw-r--r--   0        0        0      253 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3707 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1077 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/.readthedocs.yml
+-rw-r--r--   0        0        0     5226 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0     1834 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/LICENSE
+-rw-r--r--   0        0        0     3843 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/README.md
+-rw-r--r--   0        0        0       33 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/config_file.md
+-rw-r--r--   0        0        0    10368 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/index.rst
+-rw-r--r--   0        0        0     3651 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/docs/manifest.md
+-rw-r--r--   0        0        0      486 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    23074 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2794 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2187 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6751 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     2220 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/log.py
+-rw-r--r--   0        0        0    32197 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     6144 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     5956 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3423 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     6577 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/license_header.txt
+-rw-r--r--   0        0        0     1874 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/conftest.py
+-rw-r--r--   0        0        0     3118 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/test_build.py
+-rw-r--r--   0        0        0    12994 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/test_finder.py
+-rw-r--r--   0        0        0      995 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/test_manifest.py
+-rw-r--r--   0        0        0     2394 2023-05-16 09:56:32.864168 idf_build_apps-1.0.0.dev0/tests/test_utils.py
+-rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0.dev0/setup.py
+-rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0.dev0/PKG-INFO
```

### Comparing `idf-build-apps-0.6.1/.github/workflows/issue_comment.yml` & `idf_build_apps-1.0.0.dev0/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/.github/workflows/new_issues.yml` & `idf_build_apps-1.0.0.dev0/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/.github/workflows/new_prs.yml` & `idf_build_apps-1.0.0.dev0/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/.github/workflows/test-build-docs.yml` & `idf_build_apps-1.0.0.dev0/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/.github/workflows/test-build-idf-apps.yml` & `idf_build_apps-1.0.0.dev0/.github/workflows/test-build-idf-apps.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/.gitignore` & `idf_build_apps-1.0.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/.pre-commit-config.yaml` & `idf_build_apps-1.0.0.dev0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/CONTRIBUTING.md` & `idf_build_apps-1.0.0.dev0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/LICENSE` & `idf_build_apps-1.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/README.md` & `idf_build_apps-1.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/docs/Makefile` & `idf_build_apps-1.0.0.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/docs/_static/espressif-logo.svg` & `idf_build_apps-1.0.0.dev0/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/docs/_static/theme_overrides.css` & `idf_build_apps-1.0.0.dev0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/docs/conf.py` & `idf_build_apps-1.0.0.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/docs/config_file.md` & `idf_build_apps-1.0.0.dev0/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/docs/find_build.md` & `idf_build_apps-1.0.0.dev0/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/docs/manifest.md` & `idf_build_apps-1.0.0.dev0/docs/manifest.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/idf_build_apps/app.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     Manifest,
 )
 from .utils import (
     BuildError,
     find_first_match,
     rmdir,
     subprocess_run,
+    to_absolute_path,
     to_list,
 )
 
 try:
     import typing as t
 except ImportError:
     pass
@@ -122,14 +123,21 @@
             self.BUILD_SYSTEM,
             self.app_dir,
             self.target,
             self.sdkconfig_path or '(default)',
             self.build_path,
         )
 
+    def __str__(self):
+        return 'App {}, target {}, sdkconfig {}'.format(
+            self.app_dir,
+            self.target,
+            self.sdkconfig_path or '(default)',
+        )
+
     def __lt__(self, other):
         if self.app_dir != other.app_dir:
             return self.app_dir < other.app_dir
         elif self.target != other.target:
             return self.target < other.target
         else:
             return self.config_name < other.config_name
@@ -342,17 +350,24 @@
         return self._sdkconfig_files_defined_target
 
     @property
     def sdkconfig_files(self):  # type: () -> list[str]
         return [os.path.realpath(file) for file in self._sdkconfig_files]
 
     @property
-    def requires_components(self):  # type: () -> list[str]
+    def depends_components(self):  # type: () -> list[str]
         if self.MANIFEST:
-            return self.MANIFEST.requires_components(self.app_dir)
+            return self.MANIFEST.depends_components(self.app_dir)
+
+        return []
+
+    @property
+    def depends_filepatterns(self):  # type: () -> list[str]
+        if self.MANIFEST:
+            return self.MANIFEST.depends_filepatterns(self.app_dir)
 
         return []
 
     @property
     def supported_targets(self):
         if self.MANIFEST:
             return self.MANIFEST.enable_build_targets(
@@ -372,16 +387,17 @@
             )
 
         return []
 
     @abstractmethod
     def build(
         self,
-        depends_on_components=None,  # type: list[str] | str | None
+        modified_components=None,  # type: list[str] | str | None
         check_component_dependencies=False,  # type: bool
+        is_modified=False,  # type: bool
     ):  # type: (...) -> bool
         pass
 
     def write_size_json(self):
         map_file = find_first_match('*.map', self.build_path)
         if not map_file:
             LOGGER.warning(
@@ -436,14 +452,27 @@
 
         return True, is_ignored
 
     @classmethod
     def is_app(cls, path):  # type: (str) -> bool
         raise NotImplementedError('Please implement this function in sub classes')
 
+    def is_modified(self, modified_files):  # type: (list[str] | None) -> bool
+        _app_dir_fullpath = to_absolute_path(self.app_dir)
+        if modified_files:
+            for f in modified_files:
+                _f_fullpath = to_absolute_path(f)
+                if _f_fullpath.parts[-1].endswith('.md'):
+                    continue
+
+                if _app_dir_fullpath in _f_fullpath.parents:
+                    return True
+
+        return False
+
 
 class CMakeApp(App):
     BUILD_SYSTEM = 'cmake'
 
     # If these keys are present in sdkconfig.defaults, they will be extracted and passed to CMake
     SDKCONFIG_TEST_OPTS = [
         'EXCLUDE_COMPONENTS',
@@ -460,16 +489,17 @@
 
     def __init__(self, *args, **kwargs):
         self.cmake_vars = {}
         super(CMakeApp, self).__init__(*args, **kwargs)
 
     def build(
         self,
-        depends_on_components=None,  # type: list[str] | str | None
+        modified_components=None,  # type: list[str] | str | None
         check_component_dependencies=False,  # type: bool
+        is_modified=False,  # type: bool
     ):  # type: (...) -> bool
         LOGGER.debug('=> Preparing...')
         if self.work_dir != self.app_dir:
             if os.path.exists(self.work_dir):
                 LOGGER.debug('==> Work directory %s exists, removing', self.work_dir)
                 if not self.dry_run:
                     shutil.rmtree(self.work_dir)
@@ -520,33 +550,33 @@
             '-C',
             self.work_dir,
             '-DIDF_TARGET={}'.format(self.target),
             # set to ";" to disable `default` when no such variable
             '-DSDKCONFIG_DEFAULTS={}'.format(';'.join(self.sdkconfig_files) if self.sdkconfig_files else ';'),
         ]
 
-        depends_on_components = to_list(depends_on_components)
-        if depends_on_components is not None and check_component_dependencies:
+        modified_components = to_list(modified_components)
+        if modified_components is not None and check_component_dependencies and not is_modified:
             subprocess_run(
                 common_args + ['reconfigure'],
                 log_terminal=False if self.build_log_path else True,
                 log_fs=log_file,
                 check=True,
                 additional_env_dict=additional_env_dict,
             )
 
             with open(os.path.join(self.build_path, PROJECT_DESCRIPTION_JSON)) as fr:
                 build_components = set(item for item in json.load(fr)['build_components'] if item)
 
-            if not set(depends_on_components).intersection(set(build_components)):
+            if not set(modified_components).intersection(set(build_components)):
                 LOGGER.info(
-                    '=> Skip building... app %s depends on components: %s, while current build based on component dependencies: %s',
+                    '=> Skip building... app %s depends components: %s, while current build modified components: %s',
                     self.app_dir,
                     build_components,
-                    depends_on_components,
+                    modified_components,
                 )
                 return False
 
         # idf.py build
         build_args = deepcopy(common_args)
         if self.cmake_vars:
             for key, val in self.cmake_vars.items():
```

### Comparing `idf-build-apps-0.6.1/idf_build_apps/config.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 from pathlib import (
     Path,
 )
 
+from idf_build_apps.utils import (
+    to_absolute_path,
+)
+
 
 class InvalidTomlError(SystemExit):
     def __init__(self, filepath, msg):  # type: (str | Path, str) -> None
         super().__init__('Failed parsing toml file "{}" with error: {}'.format(filepath, msg))
 
 
 PYPROJECT_TOML_FN = 'pyproject.toml'
@@ -56,20 +60,20 @@
     if config is None and (dirpath / IDF_BUILD_APPS_TOML_FN).is_file():
         config, filepath = _get_config_from_file(dirpath / IDF_BUILD_APPS_TOML_FN)
 
     return config, filepath
 
 
 def get_valid_config(starts_from=os.getcwd(), custom_path=None):  # type: (str, str | None) -> dict | None
-    root_dir = Path('/').resolve()
-    cur_dir = Path(os.path.expanduser(starts_from)).resolve()
+    root_dir = to_absolute_path('/')
+    cur_dir = to_absolute_path(starts_from)
 
     config = None
     if custom_path and os.path.isfile(custom_path):
-        config, filepath = _get_config_from_file(Path(os.path.expanduser(custom_path)).resolve())
+        config, filepath = _get_config_from_file(to_absolute_path(custom_path))
         if config is not None:
             # use print here since the verbose settings may be set in the config file
             print('Using custom config file: {}'.format(filepath))
             return config
 
     while cur_dir != root_dir and config is None:
         config, filepath = _get_config_from_path(cur_dir)
```

### Comparing `idf-build-apps-0.6.1/idf_build_apps/constants.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/idf_build_apps/finder.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/finder.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from .app import (
     App,
     CMakeApp,
 )
 from .utils import (
     config_rules_from_str,
+    files_matches_patterns,
     to_list,
 )
 
 
 def _get_apps_from_path(
     path,  # type: str
     target,  # type: str
@@ -27,32 +28,48 @@
     work_dir=None,  # type: str | None
     build_dir='build',  # type: str
     config_rules_str=None,  # type: list[str] | str | None
     build_log_path=None,  # type: str | None
     size_json_path=None,  # type: str | None
     check_warnings=False,  # type: bool
     preserve=True,  # type: bool
-    depends_on_components=None,  # type: list[str] | str | None
+    manifest_rootpath=None,  # type: str | None
+    modified_components=None,  # type: list[str] | str | None
+    modified_files=None,  # type: list[str] | str | None,
     check_component_dependencies=False,  # type: bool
     sdkconfig_defaults_str=None,  # type: str | None
 ):  # type: (...) -> list[App]
-    depends_on_components = to_list(depends_on_components)
+    modified_components = to_list(modified_components)
+    modified_files = to_list(modified_files)
 
     def _validate_app(_app):  # type: (App) -> bool
         if target not in _app.supported_targets:
             LOGGER.debug('=> Skipping. %s only supports targets: %s', _app, ', '.join(_app.supported_targets))
             return False
 
-        if _app.requires_components and check_component_dependencies:
-            if not set(_app.requires_components).intersection(set(depends_on_components)):
+        if _app.is_modified(modified_files):
+            return True
+
+        if _app.depends_components and check_component_dependencies:
+            if not set(_app.depends_components).intersection(set(modified_components)):
+                LOGGER.debug(
+                    '=> Skipping. %s requires components: %s, but you passed "--modified-components %s"',
+                    _app,
+                    ', '.join(_app.depends_components),
+                    ', '.join(modified_components),
+                )
+                return False
+
+        if _app.depends_filepatterns and check_component_dependencies:
+            if not files_matches_patterns(modified_files, _app.depends_filepatterns, manifest_rootpath):
                 LOGGER.debug(
-                    '=> Skipping. %s requires components: %s, but you passed "--depends-on-components %s"',
+                    '=> Skipping. %s depends on file patterns: %s, but you passed "--modified-files %s"',
                     _app,
-                    ', '.join(_app.requires_components),
-                    ', '.join(depends_on_components),
+                    ', '.join(_app.depends_filepatterns),
+                    ', '.join(modified_files),
                 )
                 return False
 
         return True
 
     if build_system == 'cmake':
         app_cls = CMakeApp
```

### Comparing `idf-build-apps-0.6.1/idf_build_apps/log.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/idf_build_apps/main.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,42 +37,69 @@
     Manifest,
 )
 from .utils import (
     BuildError,
     InvalidCommand,
     files_matches_patterns,
     get_parallel_start_stop,
+    to_absolute_path,
     to_list,
 )
 
 try:
     import typing as t
 except ImportError:
     pass
 
 
+def _check_components_dependency(
+    manifest_rootpath,  # type: str
+    modified_components,  # type: list[str] | None
+    modified_files,  # type: list[str] | None
+    ignore_component_dependencies_file_patterns,  # type: list[str] | None
+):  # type: (...) -> bool
+    # not check since `--modified-components` is not passed
+    if modified_components is None and modified_files is None:
+        return False
+
+    # not check since `--ignore-component-dependency-file-pattern` is passed and matched
+    if (
+        ignore_component_dependencies_file_patterns
+        and modified_files
+        and files_matches_patterns(modified_files, ignore_component_dependencies_file_patterns, manifest_rootpath)
+    ):
+        LOGGER.debug(
+            'Skipping check component dependencies for apps since files %s matches patterns: %s',
+            ', '.join(modified_files),
+            ', '.join(ignore_component_dependencies_file_patterns),
+        )
+        return False
+
+    return True
+
+
 def find_apps(
     paths,  # type: list[str] | str
     target,  # type: str
     build_system='cmake',  # type: str
     recursive=False,  # type: bool
     exclude_list=None,  # type: list[str] | None
     work_dir=None,  # type: str | None
     build_dir='build',  # type: str
     config_rules_str=None,  # type: list[str] | str | None
     build_log_path=None,  # type: str | None
     size_json_path=None,  # type: str | None
     check_warnings=False,  # type: bool
     preserve=True,  # type: bool
+    manifest_rootpath=None,  # type: str | None
     manifest_files=None,  # type: list[str] | str | None
     default_build_targets=None,  # type: list[str] | str | None
-    depends_on_components=None,  # type: list[str] | str | None
-    manifest_rootpath=None,  # type: str | None
+    modified_components=None,  # type: list[str] | str | None
+    modified_files=None,  # type: list[str] | str | None
     ignore_component_dependencies_file_patterns=None,  # type: list[str] | str | None
-    depends_on_files=None,  # type: list[str] | str | None
     sdkconfig_defaults=None,  # type: str | None
 ):  # type: (...) -> list[App]
     """
     Find app directories in paths (possibly recursively), which contain apps for the given build system, compatible
     with the given target
 
     :param paths: list of app directories (can be / usually will be a relative path)
@@ -97,68 +124,53 @@
     :param size_json_path: path of the size.json file. Support placeholders.
         Will not generate size file for each app if not specified
     :type size_json_path: str | None
     :param check_warnings: Check for warnings in the build log or not
     :type check_warnings: bool
     :param preserve: Preserve the built binaries or not
     :type preserve: bool
+    :param manifest_rootpath: The root path of the manifest files. Usually the folders specified in the manifest files
+        are relative paths. Use the current directory if not specified
+    :type manifest_rootpath: str | None
     :param manifest_files: paths of the manifest files
     :type manifest_files: list[str] | str | None
     :param default_build_targets: default build targets used in manifest files
     :type default_build_targets: list[str] | str | None
-    :param depends_on_components: app with ``requires_components`` set in the corresponding manifest files will only
-        be built if it depends on any of the specified components
-    :type depends_on_components: list[str] | str | None
-    :param manifest_rootpath: The root path of the manifest files. Usually the folders specified in the manifest files
-        are relative paths. Use the current directory if not specified
-    :type manifest_rootpath: str | None
-    :param ignore_component_dependencies_file_patterns: file patterns that use to ignore checking the component
+    :param modified_components: modified components
+    :type modified_components: list[str] | str | None
+    :param modified_files: modified files
+    :type modified_files: list[str] | str | None
+    :param ignore_component_dependencies_file_patterns: file patterns that used for ignoring checking the component
         dependencies
     :type ignore_component_dependencies_file_patterns: list[str] | str | None
-    :param depends_on_files: skip check app's component dependencies if any of the specified files matches
-        ``ignore_component_dependencies_file_patterns``
-    :type depends_on_files: list[str] | str | None
     :param sdkconfig_defaults: semicolon-separated string, pass to idf.py -DSDKCONFIG_DEFAULTS if specified,
         also could be set via environment variables "SDKCONFIG_DEFAULTS"
     :type sdkconfig_defaults: str | None
     :return: list of found apps
     :rtype: list[App]
     """
     if default_build_targets:
         default_build_targets = to_list(default_build_targets)
         LOGGER.info('Overriding DEFAULT_BUILD_TARGETS to %s', default_build_targets)
         FolderRule.DEFAULT_BUILD_TARGETS = default_build_targets
 
     # always set the manifest rootpath at the very beginning of find_apps in case ESP-IDF switches the branch.
-    Manifest.ROOTPATH = Path(manifest_rootpath or os.curdir).resolve()
+    Manifest.ROOTPATH = to_absolute_path(manifest_rootpath or os.curdir)
 
     if manifest_files:
         rules = set()
         for _manifest_file in to_list(manifest_files):
             LOGGER.debug('Loading manifest file: %s', _manifest_file)
             rules.update(Manifest.from_file(_manifest_file).rules)
         manifest = Manifest(rules)
         App.MANIFEST = manifest
 
-    depends_on_components = to_list(depends_on_components)
-    if depends_on_components is None:
-        check_component_dependencies = False
-    elif (
-        ignore_component_dependencies_file_patterns
-        and depends_on_files
-        and files_matches_patterns(depends_on_files, ignore_component_dependencies_file_patterns)
-    ):
-        LOGGER.debug(
-            'Skipping check component dependencies for apps since files %s matches patterns: %s',
-            ', '.join(depends_on_files),
-            ', '.join(ignore_component_dependencies_file_patterns),
-        )
-        check_component_dependencies = False
-    else:
-        check_component_dependencies = True
+    modified_components = to_list(modified_components)
+    modified_files = to_list(modified_files)
+    ignore_component_dependencies_file_patterns = to_list(ignore_component_dependencies_file_patterns)
 
     apps = []
     if target == 'all':
         targets = ALL_TARGETS
     else:
         targets = [target]
 
@@ -174,16 +186,23 @@
                     work_dir=work_dir,
                     build_dir=build_dir or 'build',
                     config_rules_str=config_rules_str,
                     build_log_path=build_log_path,
                     size_json_path=size_json_path,
                     check_warnings=check_warnings,
                     preserve=preserve,
-                    depends_on_components=depends_on_components,
-                    check_component_dependencies=check_component_dependencies,
+                    manifest_rootpath=manifest_rootpath,
+                    modified_components=modified_components,
+                    modified_files=modified_files,
+                    check_component_dependencies=_check_components_dependency(
+                        manifest_rootpath,
+                        modified_components,
+                        modified_files,
+                        ignore_component_dependencies_file_patterns,
+                    ),
                     sdkconfig_defaults_str=sdkconfig_defaults,
                 )
             )
     apps.sort()
 
     LOGGER.info('Found %d apps in total', len(apps))
     return apps
@@ -197,18 +216,18 @@
     dry_run=False,  # type: bool
     keep_going=False,  # type: bool
     collect_size_info=None,  # type: str | t.TextIO | None
     collect_app_info=None,  # type: str | t.TextIO | None
     ignore_warning_strs=None,  # type: list[str] | None
     ignore_warning_file=None,  # type: t.TextIO | None
     copy_sdkconfig=False,  # type: bool
-    depends_on_components=None,  # type: list[str] | str | None
     manifest_rootpath=None,  # type: str | None
+    modified_components=None,  # type: list[str] | str | None
+    modified_files=None,  # type: list[str] | str | None
     ignore_component_dependencies_file_patterns=None,  # type: list[str] | str | None
-    depends_on_files=None,  # type: list[str] | str | None
 ):  # type: (...) -> (int, list[App]) | int
     """
     Build all the specified apps
 
     :param apps: list of apps to be built
     :type apps: list[App] | App
     :param build_verbose: call ``--verbose`` in ``idf.py build`` or not
@@ -228,62 +247,43 @@
     :param ignore_warning_strs: ignore build warnings that matches any of the specified regex patterns
     :type ignore_warning_strs: list[str] | None
     :param ignore_warning_file: ignore build warnings that matches any of the lines of the regex patterns in the
         specified file
     :type ignore_warning_file: list[str] | None
     :param copy_sdkconfig: copy the sdkconfig file to the build directory or not
     :type copy_sdkconfig: bool
-    :param depends_on_components: app with ``requires_components`` set in the corresponding manifest files would only be
-        built if it depends on any of the specified components
-    :type depends_on_components: list[str] | str | None
     :param manifest_rootpath: The root path of the manifest files. Usually the folders specified in the manifest files
         are relative paths. Use the current directory if not specified
     :type manifest_rootpath: str | None
-    :param ignore_component_dependencies_file_patterns: file patterns that use to ignore checking the component
+    :param modified_components: modified components
+    :type modified_components: list[str] | str | None
+    :param modified_files: modified files
+    :type modified_files: list[str] | str | None
+    :param ignore_component_dependencies_file_patterns: file patterns that used for ignoring checking the component
         dependencies
     :type ignore_component_dependencies_file_patterns: list[str] | str | None
-    :param depends_on_files: skip check app's component dependencies if any of the specified files matches
-        ``ignore_component_dependencies_file_patterns``
-    :type depends_on_files: list[str] | str | None
-    :return: exit_code, built_apps if specified ``depends_on_components``
+    :return: (exit_code, built_apps) if specified ``modified_components``
     :rtype: int, list[App]
-    :return: exit_code if not specified ``depends_on_components``
+    :return: exit_code if not specified ``modified_components``
     :rtype: int
     """
     apps = to_list(apps)  # type: list[App]
+    modified_components = to_list(modified_components)
+    modified_files = to_list(modified_files)
+    ignore_component_dependencies_file_patterns = to_list(ignore_component_dependencies_file_patterns)
 
     ignore_warnings_regexes = []
     if ignore_warning_strs:
         for s in ignore_warning_strs:
             ignore_warnings_regexes.append(re.compile(s))
     if ignore_warning_file:
         for s in ignore_warning_file:
             ignore_warnings_regexes.append(re.compile(s.strip()))
     App.IGNORE_WARNS_REGEXES = ignore_warnings_regexes
 
-    depends_on_components = to_list(depends_on_components)
-    # here depends_on_components [''] means that the user use --depends-on-components
-    # the ones with `requires_components` are already been filtered out
-    # if we skip all build, that would be too aggressive
-    if depends_on_components is None or depends_on_components == ['']:
-        check_component_dependencies = False
-    elif (
-        ignore_component_dependencies_file_patterns
-        and depends_on_files
-        and files_matches_patterns(depends_on_files, ignore_component_dependencies_file_patterns, manifest_rootpath)
-    ):
-        LOGGER.debug(
-            'Skipping check component dependencies for apps since files %s matches patterns: %s',
-            ', '.join(depends_on_files),
-            ', '.join(ignore_component_dependencies_file_patterns),
-        )
-        check_component_dependencies = False
-    else:
-        check_component_dependencies = True
-
     start, stop = get_parallel_start_stop(len(apps), parallel_count, parallel_index)
     LOGGER.info('Total %s apps. running build for app %s-%s', len(apps), start, stop)
 
     failed_apps = []
     exit_code = 0
 
     LOGGER.info('Building the following apps:')
@@ -328,43 +328,53 @@
     for f in collect_files:
         if os.path.isfile(f):
             os.remove(f)
             LOGGER.info('=> Remove existing collect file %s', f)
         Path(f).touch()
 
     actual_built_apps = []
+    built_apps = []  # type: list[App]
+    skipped_apps = []  # type: list[App]
     for i, app in enumerate(apps):
         index = i + 1  # we use 1-based
         if index < start or index > stop:
             continue
 
         # attrs
         app.dry_run = dry_run
         app.index = index
         app.verbose = build_verbose
 
         LOGGER.info('Building app %s: %s', index, repr(app))
         is_built = False
         try:
             is_built = app.build(
-                depends_on_components=depends_on_components,
-                check_component_dependencies=check_component_dependencies,
+                modified_components=modified_components,
+                check_component_dependencies=_check_components_dependency(
+                    manifest_rootpath, modified_components, modified_files, ignore_component_dependencies_file_patterns
+                ),
+                is_modified=app.is_modified(modified_files),
             )
         except BuildError as e:
             LOGGER.error(str(e))
             if keep_going:
                 failed_apps.append(app)
                 exit_code = 1
             else:
-                if depends_on_components is not None:
+                if modified_components is not None:
                     return 1, actual_built_apps
                 else:
                     return 1
         finally:
             if is_built:
+                built_apps.append(app)
+            else:
+                skipped_apps.append(app)
+
+            if is_built:
                 actual_built_apps.append(app)
 
                 if app.collect_app_info:
                     with open(app.collect_app_info, 'a') as fw:
                         fw.write(app.to_json() + '\n')
                     LOGGER.info('=> Recorded app info in %s', app.collect_app_info)
 
@@ -401,20 +411,30 @@
                         LOGGER.warning(e)
                         pass
                     else:
                         LOGGER.info('=> Copied sdkconfig file from %s to %s', app.work_dir, app.build_path)
 
             LOGGER.info('')  # add one empty line for separating different builds
 
+    if built_apps:
+        LOGGER.info('Built the following apps:')
+        for app in built_apps:
+            LOGGER.info('  %s', app)
+
+    if skipped_apps:
+        LOGGER.info('Skipped the following apps:')
+        for app in skipped_apps:
+            LOGGER.info('  %s', app)
+
     if failed_apps:
         LOGGER.error('Build failed for the following apps:')
         for app in failed_apps:
             LOGGER.error('  %s', app)
 
-    if depends_on_components is not None:
+    if modified_components is not None:
         return exit_code, actual_built_apps
     else:
         return exit_code
 
 
 class IdfBuildAppsCliFormatter(argparse.HelpFormatter):
     LINE_SEP = '$LINE_SEP$'
@@ -571,36 +591,39 @@
         help='space-separated list of supported targets. Targets supported in current ESP-IDF branch '
         '(except preview ones) would be used if this option is not set.'
         '{} ! DeprecationWarning: comma-separated list support will be removed in idf-build-apps 1.0.0 version'.format(
             IdfBuildAppsCliFormatter.LINE_SEP
         ),
     )
     common_args.add_argument(
-        '--depends-on-components',
+        '--modified-components',
         nargs='*',
         default=None,
-        help='space-separated components list, app with `requires_components` set in the corresponding manifest files '
-        'would only be built if depends on any of the specified components',
+        help='space-separated list which specifies the modified components. app with `depends_components` set in the '
+        'corresponding manifest files would only be built if depends on any of the specified components.',
     )
     common_args.add_argument(
-        '-if',
-        '--ignore-component-dependencies-file-patterns',
+        '--modified-files',
         nargs='*',
         default=None,
-        help='ignore component dependencies when changed files matches any of the specified file patterns. must used '
-        'with --depends-on-files',
+        help='space-separated list which specifies the modified files. app with `depends_filepatterns` set in the '
+        'corresponding manifest files would only be built if any of the specified file pattern matches any of the '
+        'specified modified files.',
     )
     common_args.add_argument(
-        '--depends-on-files',
+        '-if',
+        '--ignore-component-dependencies-file-patterns',
         nargs='*',
         default=None,
-        help='space-separated file pattern list, the `requires_components` set in the manifest files will be '
-        'ignored when specified files match any of the specified file patterns defined with '
-        '--ignore-component-dependencies-file-patterns. Must used with --ignore-component-dependencies-file-patterns',
+        help='space-separated list which specifies the file patterns used for ignoring the component dependencies. '
+        'The `depends_components` and `depends_filepatterns` set in the manifest files will be ignored when any of '
+        'the specified file patterns matches any of the modified files. Must be used together with '
+        '--modified-files',
     )
+
     common_args.add_argument(
         '--no-color',
         action='store_true',
         help='enable colored output by default on UNIX-like systems. enable this flag to make the logs uncolored.',
     )
 
     find_parser = actions.add_parser('find', parents=[common_args], formatter_class=IdfBuildAppsCliFormatter)
@@ -697,19 +720,19 @@
                     )
 
                 if _t not in default_build_targets:
                     default_build_targets.append(_t)
 
     args.default_build_targets = default_build_targets
 
-    if (args.ignore_component_dependencies_file_patterns is None) != (args.depends_on_files is None):
-        raise InvalidCommand(
-            'Must specify both "--ignore-component-dependencies-file-patterns" and "--depends-on-files" '
-            'or neither of them'
-        )
+    if args.ignore_component_dependencies_file_patterns:
+        if args.modified_files is None:
+            raise InvalidCommand(
+                'Must specify "--ignore-component-dependencies-file-patterns" with "--modified-files", '
+            )
 
 
 def apply_config_args(args):  # type: (argparse.Namespace) -> None
     # support toml config file
     config_dict = get_valid_config(custom_path=args.config_file)
     if config_dict:
         for k, v in config_dict.items():
@@ -734,20 +757,20 @@
         exclude_list=args.exclude or [],
         work_dir=args.work_dir,
         build_dir=args.build_dir or 'build',
         config_rules_str=args.config,
         build_log_path=args.build_log,
         size_json_path=args.size_file,
         check_warnings=args.check_warnings,
+        manifest_rootpath=args.manifest_rootpath,
         manifest_files=args.manifest_file,
         default_build_targets=args.default_build_targets,
-        depends_on_components=args.depends_on_components,
-        manifest_rootpath=args.manifest_rootpath,
+        modified_components=args.modified_components,
+        modified_files=args.modified_files,
         ignore_component_dependencies_file_patterns=args.ignore_component_dependencies_file_patterns,
-        depends_on_files=args.depends_on_files,
         sdkconfig_defaults=args.sdkconfig_defaults,
     )
 
     if args.action == 'find':
         if args.output:
             with open(args.output, 'w') as f:
                 for app in apps:
@@ -770,17 +793,17 @@
         dry_run=args.dry_run,
         keep_going=args.keep_going,
         collect_size_info=args.collect_size_info,
         collect_app_info=args.collect_app_info,
         ignore_warning_strs=args.ignore_warning_str,
         ignore_warning_file=args.ignore_warning_file,
         copy_sdkconfig=args.copy_sdkconfig,
-        depends_on_components=args.depends_on_components,
         manifest_rootpath=args.manifest_rootpath,
+        modified_components=args.modified_components,
+        modified_files=args.modified_files,
         ignore_component_dependencies_file_patterns=args.ignore_component_dependencies_file_patterns,
-        depends_on_files=args.depends_on_files,
     )
 
-    if args.depends_on_components is not None:
+    if args.modified_components is not None:
         sys.exit(res[0])
     else:
         sys.exit(res)
```

### Comparing `idf-build-apps-0.6.1/idf_build_apps/manifest/if_parser.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/if_parser.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/idf_build_apps/manifest/manifest.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/manifest.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,28 +39,30 @@
 
     def __init__(
         self,
         folder,  # type: Path
         enable=None,  # type: list[dict[str, str]] | None
         disable=None,  # type: list[dict[str, str]] | None
         disable_test=None,  # type: list[dict[str, str]] | None
-        requires_components=None,  # type: list[str] | None
+        depends_components=None,  # type: list[str] | None
+        depends_filepatterns=None,  # type: list[str] | None
     ):  # type: (...) -> None
         self.folder = folder.resolve()
 
         for group in [enable, disable, disable_test]:
             if group:
                 for d in group:
                     d['stmt'] = d['if']  # avoid keyword `if`
                     del d['if']
 
         self.enable = [IfClause(**clause) for clause in enable] if enable else []
         self.disable = [IfClause(**clause) for clause in disable] if disable else []
         self.disable_test = [IfClause(**clause) for clause in disable_test] if disable_test else []
-        self.requires_components = requires_components or []
+        self.depends_components = depends_components or []
+        self.depends_filepatterns = depends_filepatterns or []
 
     def __hash__(self):
         return hash(self.folder)
 
     def __repr__(self):
         return 'FolderRule({})'.format(self.folder)
 
@@ -164,9 +166,12 @@
         return self._most_suitable_rule(folder).enable_build_targets(default_sdkconfig_target, config_name)
 
     def enable_test_targets(
         self, folder, default_sdkconfig_target=None, config_name=None
     ):  # type: (str, str | None, str | None) -> list[str]
         return self._most_suitable_rule(folder).enable_test_targets(default_sdkconfig_target, config_name)
 
-    def requires_components(self, folder):  # type: (str) -> list[str]
-        return self._most_suitable_rule(folder).requires_components
+    def depends_components(self, folder):  # type: (str) -> list[str]
+        return self._most_suitable_rule(folder).depends_components
+
+    def depends_filepatterns(self, folder):  # type: (str) -> list[str]
+        return self._most_suitable_rule(folder).depends_filepatterns
```

### Comparing `idf-build-apps-0.6.1/idf_build_apps/manifest/soc_header.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/idf_build_apps/utils.py` & `idf_build_apps-1.0.0.dev0/idf_build_apps/utils.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/pyproject.toml` & `idf_build_apps-1.0.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/tests/conftest.py` & `idf_build_apps-1.0.0.dev0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 @pytest.fixture(autouse=True)
 def clean_cls_attr():
     App.MANIFEST = None
 
 
 @pytest.fixture(autouse=True)
 def setup_logging_debug():
-    setup_logging(2)
+    setup_logging(1)
 
 
 def create_project(name, folder):
     p = str(folder / name)
     os.makedirs(p)
     os.makedirs(os.path.join(p, 'main'))
```

### Comparing `idf-build-apps-0.6.1/tests/test_build.py` & `idf_build_apps-1.0.0.dev0/tests/test_build.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,43 +20,70 @@
         CMakeApp(str(path), 'esp32', work_dir=str(tmpdir / 'test')).build()
 
         captured = capsys.readouterr()
         assert 'Configuring done' in captured.out
         assert 'Project build complete.' in captured.out
 
     @pytest.mark.parametrize(
-        'depends_on_components, check_component_dependencies, assert_build_done',
+        'modified_components, check_component_dependencies, assert_build_done',
         [
             (None, True, True),
             ([], True, False),
             ([], False, True),
             ('fake', True, False),
             ('fake', False, True),
             ('soc', True, True),
             ('soc', False, True),
             (['soc', 'fake'], True, True),
         ],
     )
-    def test_build_with_depends_on_components(
-        self, tmpdir, capsys, depends_on_components, check_component_dependencies, assert_build_done
+    def test_build_with_modified_components(
+        self, tmpdir, capsys, modified_components, check_component_dependencies, assert_build_done
     ):
         path = IDF_PATH / 'examples' / 'get-started' / 'hello_world'
 
         CMakeApp(str(path), 'esp32', work_dir=str(tmpdir / 'test')).build(
-            depends_on_components=depends_on_components,
+            modified_components=modified_components,
             check_component_dependencies=check_component_dependencies,
         )
 
         captured = capsys.readouterr()
         assert 'Configuring done' in captured.out
         if assert_build_done:
             assert 'Project build complete.' in captured.out
         else:
             assert 'Project build complete.' not in captured.out
 
+    @pytest.mark.parametrize(
+        'modified_files, is_built',
+        [
+            ('/foo', False),
+            (str(IDF_PATH / 'examples' / 'README.md'), False),
+            ([str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], False),
+            (
+                [
+                    str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md'),
+                    str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.c'),
+                ],
+                True,
+            ),
+        ],
+    )
+    def test_build_with_modified_files(self, modified_files, is_built):
+        test_dir = str(IDF_PATH / 'examples' / 'get-started' / 'hello_world')
+
+        app = CMakeApp(test_dir, 'esp32')
+        built = app.build(
+            modified_components=[],
+            check_component_dependencies=True,
+            is_modified=app.is_modified(modified_files),
+        )
+
+        assert built == is_built
+
 
 @pytest.mark.skipif(not shutil.which('idf.py'), reason='idf.py not found')
 def test_idf_version_keywords_type():
     from idf_build_apps.constants import (
         IDF_VERSION_MAJOR,
         IDF_VERSION_MINOR,
         IDF_VERSION_PATCH,
```

### Comparing `idf-build-apps-0.6.1/tests/test_finder.py` & `idf_build_apps-1.0.0.dev0/tests/test_finder.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,45 +98,133 @@
         - if: IDF_VERSION_MAJOR > 0 and IDF_VERSION_MINOR < 999 and IDF_VERSION_PATCH in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
 ''',
             encoding='utf8',
         )
         assert find_apps(str(test_dir), 'esp32', recursive=True, manifest_files=str(yaml_file)) == apps
 
     @pytest.mark.parametrize(
-        'depends_on_components, could_find_apps',
+        'modified_components, could_find_apps',
         [
             (None, True),
             ([], False),
             ('fake', False),
             ('soc', True),
             (['soc', 'fake'], True),
         ],
     )
-    def test_with_requires_and_depends_on_components(self, tmpdir, depends_on_components, could_find_apps):
+    def test_with_requires_and_modified_components(self, tmpdir, modified_components, could_find_apps):
         test_dir = str(IDF_PATH / 'examples')
         apps = find_apps(test_dir, 'esp32', recursive=True)
         assert apps
 
         yaml_file = tmpdir / 'test.yml'
         yaml_file.write_text(
             f'''
 {test_dir}:
-    requires_components:
+    depends_components:
         - freertos
         - soc
 ''',
             encoding='utf8',
         )
 
         filtered_apps = find_apps(
             test_dir,
             'esp32',
             recursive=True,
             manifest_files=yaml_file,
-            depends_on_components=depends_on_components,
+            modified_components=modified_components,
+        )
+        if could_find_apps:
+            assert filtered_apps == apps
+        else:
+            assert not filtered_apps
+
+    @pytest.mark.parametrize(
+        'modified_files, could_find_apps',
+        [
+            ('/foo', False),
+            (str(IDF_PATH / 'examples' / 'README.md'), False),
+            ([str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], False),
+            (
+                [
+                    str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md'),
+                    str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.c'),
+                ],
+                True,
+            ),
+        ],
+    )
+    def test_with_depends_components_but_modified(self, tmp_path, modified_files, could_find_apps):
+        test_dir = str(IDF_PATH / 'examples' / 'get-started' / 'hello_world')
+        apps = find_apps(test_dir, 'esp32', recursive=True)
+        assert apps
+
+        yaml_file = tmp_path / 'test.yml'
+        yaml_file.write_text(
+            f'''
+{test_dir}:
+    depends_components:
+        - soc
+''',
+            encoding='utf8',
+        )
+
+        filtered_apps = find_apps(
+            test_dir,
+            'esp32',
+            recursive=True,
+            manifest_files=yaml_file,
+            modified_components=[],
+            modified_files=modified_files,
+        )
+        if could_find_apps:
+            assert filtered_apps == apps
+        else:
+            assert not filtered_apps
+
+    @pytest.mark.parametrize(
+        'modified_files, could_find_apps',
+        [
+            ('/foo', True),
+            (str(IDF_PATH / 'examples' / 'README.md'), False),
+            ([str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], True),
+            (
+                [
+                    str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md'),
+                    str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.c'),
+                ],
+                True,
+            ),
+        ],
+    )
+    def test_with_depends_filepatterns(self, tmp_path, modified_files, could_find_apps):
+        test_dir = str(IDF_PATH / 'examples' / 'get-started' / 'hello_world')
+        apps = find_apps(test_dir, 'esp32', recursive=True)
+        assert apps
+
+        yaml_file = tmp_path / 'test.yml'
+        yaml_file.write_text(
+            f'''
+{test_dir}:
+    depends_filepatterns:
+        - /foo
+        - examples/get-started/hello_world/**
+        - examples/foo/**
+''',
+            encoding='utf8',
+        )
+
+        filtered_apps = find_apps(
+            test_dir,
+            'esp32',
+            recursive=True,
+            manifest_rootpath=str(IDF_PATH),
+            manifest_files=yaml_file,
+            modified_files=modified_files,
         )
         if could_find_apps:
             assert filtered_apps == apps
         else:
             assert not filtered_apps
```

### Comparing `idf-build-apps-0.6.1/tests/test_manifest.py` & `idf_build_apps-1.0.0.dev0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/tests/test_utils.py` & `idf_build_apps-1.0.0.dev0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.1/setup.py` & `idf_build_apps-1.0.0.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='0.6.1',
+      version='1.0.0.dev0',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf-build-apps-0.6.1/PKG-INFO` & `idf_build_apps-1.0.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 0.6.1
+Version: 1.0.0.dev0
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
```

