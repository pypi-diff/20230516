# Comparing `tmp/dvc-render-0.5.0.tar.gz` & `tmp/dvc-render-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-render-0.5.0.tar", last modified: Mon May 15 17:37:03 2023, max compression
+gzip compressed data, was "dvc-render-0.5.1.tar", last modified: Tue May 16 14:26:10 2023, max compression
```

## Comparing `dvc-render-0.5.0.tar` & `dvc-render-0.5.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.766903 dvc-render-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-15 17:36:41.000000 dvc-render-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-15 17:36:41.000000 dvc-render-0.5.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-15 17:36:41.000000 dvc-render-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-15 17:36:41.000000 dvc-render-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-15 17:37:03.766903 dvc-render-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-15 17:36:41.000000 dvc-render-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-15 17:36:41.000000 dvc-render-0.5.0/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 17:36:41.000000 dvc-render-0.5.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 17:36:41.000000 dvc-render-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-15 17:36:41.000000 dvc-render-0.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-15 17:36:41.000000 dvc-render-0.5.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-15 17:36:41.000000 dvc-render-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-15 17:37:03.766903 dvc-render-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.762903 dvc-render-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.766903 dvc-render-0.5.0/src/dvc_render/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/plotly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/vega.py
--rw-r--r--   0 runner    (1001) docker     (123)    23900 2023-05-15 17:36:41.000000 dvc-render-0.5.0/src/dvc_render/vega_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.766903 dvc-render-0.5.0/src/dvc_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 17:37:03.000000 dvc-render-0.5.0/src/dvc_render.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:37:03.766903 dvc-render-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-15 17:36:41.000000 dvc-render-0.5.0/tests/test_vega.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:26:10.006151 dvc-render-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-16 14:25:48.000000 dvc-render-0.5.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 14:25:48.000000 dvc-render-0.5.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:26:10.002151 dvc-render-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-16 14:25:48.000000 dvc-render-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:26:10.002151 dvc-render-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 14:25:48.000000 dvc-render-0.5.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-16 14:25:48.000000 dvc-render-0.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-16 14:25:48.000000 dvc-render-0.5.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 14:25:48.000000 dvc-render-0.5.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 14:25:48.000000 dvc-render-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-16 14:25:48.000000 dvc-render-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-16 14:25:48.000000 dvc-render-0.5.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-16 14:25:48.000000 dvc-render-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-16 14:25:48.000000 dvc-render-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-16 14:26:10.006151 dvc-render-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-16 14:25:48.000000 dvc-render-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:26:10.002151 dvc-render-0.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:26:10.002151 dvc-render-0.5.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-16 14:25:48.000000 dvc-render-0.5.1/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-16 14:25:48.000000 dvc-render-0.5.1/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 14:25:48.000000 dvc-render-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-16 14:25:48.000000 dvc-render-0.5.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-16 14:25:48.000000 dvc-render-0.5.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-16 14:25:48.000000 dvc-render-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-16 14:26:10.006151 dvc-render-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:26:10.002151 dvc-render-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:26:10.006151 dvc-render-0.5.1/src/dvc_render/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/vega.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-05-16 14:25:48.000000 dvc-render-0.5.1/src/dvc_render/vega_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:26:10.006151 dvc-render-0.5.1/src/dvc_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-16 14:26:09.000000 dvc-render-0.5.1/src/dvc_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-16 14:26:09.000000 dvc-render-0.5.1/src/dvc_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:26:09.000000 dvc-render-0.5.1/src/dvc_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:26:09.000000 dvc-render-0.5.1/src/dvc_render.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-16 14:26:09.000000 dvc-render-0.5.1/src/dvc_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 14:26:09.000000 dvc-render-0.5.1/src/dvc_render.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:26:10.006151 dvc-render-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:25:48.000000 dvc-render-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-16 14:25:48.000000 dvc-render-0.5.1/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-16 14:25:48.000000 dvc-render-0.5.1/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-16 14:25:48.000000 dvc-render-0.5.1/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-16 14:25:48.000000 dvc-render-0.5.1/tests/test_parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-16 14:25:48.000000 dvc-render-0.5.1/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-16 14:25:48.000000 dvc-render-0.5.1/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-16 14:25:48.000000 dvc-render-0.5.1/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-16 14:25:48.000000 dvc-render-0.5.1/tests/test_vega.py
```

### Comparing `dvc-render-0.5.0/.cruft.json` & `dvc-render-0.5.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/.github/dependabot.yml` & `dvc-render-0.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/.github/workflows/docs.yml` & `dvc-render-0.5.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/.github/workflows/release.yml` & `dvc-render-0.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/.github/workflows/tests.yml` & `dvc-render-0.5.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/.gitignore` & `dvc-render-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/.pre-commit-config.yaml` & `dvc-render-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/CODE_OF_CONDUCT.rst` & `dvc-render-0.5.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/CONTRIBUTING.rst` & `dvc-render-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/LICENSE` & `dvc-render-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/PKG-INFO` & `dvc-render-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-render
-Version: 0.5.0
+Version: 0.5.1
 Summary: DVC render
 Home-page: https://github.com/iterative/dvc-render
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-render-0.5.0/README.rst` & `dvc-render-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/docs/assets/logo.svg` & `dvc-render-0.5.1/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/docs/gen_ref_pages.py` & `dvc-render-0.5.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/mkdocs.yml` & `dvc-render-0.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/noxfile.py` & `dvc-render-0.5.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/pyproject.toml` & `dvc-render-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/setup.cfg` & `dvc-render-0.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 	mkdocs-section-index==0.3.4
 	mkdocstrings-python==0.7.1
 tests = 
 	%(table)s
 	%(markdown)s
 	funcy>=1.17
 	pytest==7.2.0
-	pytest-sugar==0.9.5
+	pytest-sugar>=0.9.6,<1.0
 	pytest-cov==3.0.0
 	pytest-mock==3.8.2
 	pylint==2.15.0
 	mypy==0.981
 	pytest-test-utils>=0.0.6
 dev = 
 	%(table)s
```

### Comparing `dvc-render-0.5.0/src/dvc_render/base.py` & `dvc-render-0.5.1/src/dvc_render/base.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/src/dvc_render/html.py` & `dvc-render-0.5.1/src/dvc_render/html.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/src/dvc_render/image.py` & `dvc-render-0.5.1/src/dvc_render/image.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/src/dvc_render/markdown.py` & `dvc-render-0.5.1/src/dvc_render/markdown.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/src/dvc_render/plotly.py` & `dvc-render-0.5.1/src/dvc_render/plotly.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/src/dvc_render/table.py` & `dvc-render-0.5.1/src/dvc_render/table.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/src/dvc_render/vega.py` & `dvc-render-0.5.1/src/dvc_render/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/src/dvc_render/vega_templates.py` & `dvc-render-0.5.1/src/dvc_render/vega_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         x.append(e)
     return x
 
 
 def dict_find_value(d: dict, value: str) -> bool:
     for v in d.values():
         if isinstance(v, dict):
-            return dict_find_value(v, value)
+            if dict_find_value(v, value):
+                return True
         if isinstance(v, str):
             if v == value:
                 return True
     return False
 
 
 class Template:
```

### Comparing `dvc-render-0.5.0/src/dvc_render.egg-info/PKG-INFO` & `dvc-render-0.5.1/src/dvc_render.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-render
-Version: 0.5.0
+Version: 0.5.1
 Summary: DVC render
 Home-page: https://github.com/iterative/dvc-render
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-render-0.5.0/src/dvc_render.egg-info/SOURCES.txt` & `dvc-render-0.5.1/src/dvc_render.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/src/dvc_render.egg-info/requires.txt` & `dvc-render-0.5.1/src/dvc_render.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [dev]
 tabulate>=0.8.7
 flatten_dict<1,>=0.4.1
 matplotlib
 funcy>=1.17
 pytest==7.2.0
-pytest-sugar==0.9.5
+pytest-sugar<1.0,>=0.9.6
 pytest-cov==3.0.0
 pytest-mock==3.8.2
 pylint==2.15.0
 mypy==0.981
 pytest-test-utils>=0.0.6
 mkdocs==1.3.1
 mkdocs-gen-files==0.3.5
@@ -35,13 +35,13 @@
 
 [tests]
 tabulate>=0.8.7
 flatten_dict<1,>=0.4.1
 matplotlib
 funcy>=1.17
 pytest==7.2.0
-pytest-sugar==0.9.5
+pytest-sugar<1.0,>=0.9.6
 pytest-cov==3.0.0
 pytest-mock==3.8.2
 pylint==2.15.0
 mypy==0.981
 pytest-test-utils>=0.0.6
```

### Comparing `dvc-render-0.5.0/tests/test_html.py` & `dvc-render-0.5.1/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/tests/test_image.py` & `dvc-render-0.5.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/tests/test_markdown.py` & `dvc-render-0.5.1/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/tests/test_parallel_coordinates.py` & `dvc-render-0.5.1/tests/test_parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/tests/test_table.py` & `dvc-render-0.5.1/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/tests/test_templates.py` & `dvc-render-0.5.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.0/tests/test_vega.py` & `dvc-render-0.5.1/tests/test_vega.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 import pytest
 
 from dvc_render.vega import BadTemplateError, VegaRenderer
 from dvc_render.vega_templates import NoFieldInDataError, Template
 
 # pylint: disable=missing-function-docstring, C1803
 
@@ -99,19 +101,37 @@
         "actual",
         "predicted",
     ]
     assert plot_content["spec"]["encoding"]["x"]["field"] == "predicted"
     assert plot_content["spec"]["encoding"]["y"]["field"] == "actual"
 
 
-def test_bad_template():
+def test_bad_template_on_init():
     with pytest.raises(BadTemplateError):
         Template("name", "content")
 
 
+def test_bad_template_on_missing_data(tmp_dir):
+    template_content = {"data": {"values": "BAD_ANCHOR"}}
+    tmp_dir.gen("bar.json", json.dumps(template_content))
+    datapoints = [{"val": 2}, {"val": 3}]
+    renderer = VegaRenderer(datapoints, "foo", template="bar.json")
+
+    with pytest.raises(BadTemplateError):
+        renderer.get_filled_template()
+
+    template_content = {
+        "mark": {"type": "bar"},
+        "data": {"values": Template.anchor("data")},
+    }
+    tmp_dir.gen("bar.json", json.dumps(template_content))
+    renderer = VegaRenderer(datapoints, "foo", template="bar.json")
+    assert renderer.get_filled_template()
+
+
 def test_raise_on_wrong_field():
     datapoints = [{"val": 2}, {"val": 3}]
     props = {"x": "no_val"}
     renderer = VegaRenderer(datapoints, "foo", **props)
     with pytest.raises(NoFieldInDataError):
         renderer.get_filled_template()
     renderer.get_filled_template(strict=False)
```

