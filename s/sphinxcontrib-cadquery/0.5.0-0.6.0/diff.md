# Comparing `tmp/sphinxcontrib_cadquery-0.5.0.tar.gz` & `tmp/sphinxcontrib_cadquery-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_cadquery-0.5.0.tar", max compression
+gzip compressed data, was "sphinxcontrib_cadquery-0.6.0.tar", max compression
```

## Comparing `sphinxcontrib_cadquery-0.5.0.tar` & `sphinxcontrib_cadquery-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1092 2023-03-05 00:39:01.556605 sphinxcontrib_cadquery-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      611 2023-01-05 04:01:57.599868 sphinxcontrib_cadquery-0.5.0/LICENSE
--rw-r--r--   0        0        0     1490 2023-01-05 04:03:49.236254 sphinxcontrib_cadquery-0.5.0/LICENSE.vtk-js
--rw-r--r--   0        0        0      915 2023-01-21 05:16:25.764896 sphinxcontrib_cadquery-0.5.0/README.rst
--rw-r--r--   0        0        0     2719 2023-03-05 00:38:29.824616 sphinxcontrib_cadquery-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1975 2023-03-05 00:38:29.804616 sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/__init__.py
--rw-r--r--   0        0        0     6336 2023-01-28 21:04:39.449485 sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/cq_core.py
--rw-r--r--   0        0        0     1289 2023-03-05 00:20:28.993334 sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/static/cadquery.css
--rw-r--r--   0        0        0  2267604 2023-01-05 11:41:56.759400 sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/static/dist/vtk-lite.js
--rw-r--r--   0        0        0       66 2023-01-05 11:41:56.759400 sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/static/dist/vtk-lite.js.LICENSE.txt
--rw-r--r--   0        0        0     4845 2023-01-12 08:55:03.528651 sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/static/render.js
--rw-r--r--   0        0        0      653 2023-03-05 00:20:28.997334 sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/templates/svg.rst.jinja
--rw-r--r--   0        0        0     1301 2023-03-05 00:20:28.997334 sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/templates/vtk.rst.jinja
--rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 sphinxcontrib_cadquery-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1196 2023-05-16 12:19:09.080555 sphinxcontrib_cadquery-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      611 2023-01-05 04:01:57.599868 sphinxcontrib_cadquery-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1490 2023-01-05 04:03:49.236254 sphinxcontrib_cadquery-0.6.0/LICENSE.vtk-js
+-rw-r--r--   0        0        0      915 2023-01-21 05:16:25.764896 sphinxcontrib_cadquery-0.6.0/README.rst
+-rw-r--r--   0        0        0     2725 2023-05-16 12:18:21.888425 sphinxcontrib_cadquery-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1975 2023-05-16 12:18:21.868425 sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/__init__.py
+-rw-r--r--   0        0        0     6336 2023-01-28 21:04:39.449485 sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/cq_core.py
+-rw-r--r--   0        0        0     1317 2023-05-07 00:57:15.044268 sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/static/cadquery.css
+-rw-r--r--   0        0        0  2267604 2023-01-05 11:41:56.759400 sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/static/dist/vtk-lite.js
+-rw-r--r--   0        0        0       66 2023-01-05 11:41:56.759400 sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/static/dist/vtk-lite.js.LICENSE.txt
+-rw-r--r--   0        0        0     4845 2023-01-12 08:55:03.528651 sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/static/render.js
+-rw-r--r--   0        0        0      653 2023-03-05 00:20:28.997334 sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/templates/svg.rst.jinja
+-rw-r--r--   0        0        0     1278 2023-05-07 00:57:15.044268 sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/templates/vtk.rst.jinja
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 sphinxcontrib_cadquery-0.6.0/PKG-INFO
```

### Comparing `sphinxcontrib_cadquery-0.5.0/CHANGELOG.md` & `sphinxcontrib_cadquery-0.6.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## 0.6.0 (2023-05-17)
+
+### Feat
+
+- add border around svg image
+
+### Fix
+
+- allow sphinx >=5.3.0,<7.0.0
+
 ## 0.5.0 (2023-03-05)
 
 ### Feat
 
 - vtk.js navigation legend
 
 ## 0.4.0 (2023-01-29)
```

### Comparing `sphinxcontrib_cadquery-0.5.0/LICENSE` & `sphinxcontrib_cadquery-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_cadquery-0.5.0/LICENSE.vtk-js` & `sphinxcontrib_cadquery-0.6.0/LICENSE.vtk-js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_cadquery-0.5.0/README.rst` & `sphinxcontrib_cadquery-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_cadquery-0.5.0/pyproject.toml` & `sphinxcontrib_cadquery-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxcontrib-cadquery"
-version = "0.5.0"
+version = "0.6.0"
 description = "Sphinx extension for rendering CadQuery models."
 packages = [
     {include = "sphinxcontrib"},
 ]
 include = [
     "CHANGELOG.md",
     "sphinxcontrib/cadquery/static/dist/vtk-lite.js*",
@@ -52,24 +52,24 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/sethfischer/sphinxcontrib-cadquery/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 
-Sphinx = "^5.3.0"
+Sphinx = ">=5.3.0,<7.0.0"
 ipython = ">=7.31.1"
 jinja2 = ">=3.0"
 
 [tool.poetry.group.dev.dependencies]
 cadquery = "^2.2.0"
 casadi = {version = "^3.5.6rc2", allow-prereleases = true}
 
-black = "^22.12.0"
-commitizen = "^2.39.1"
+black = "^23.3.0"
+commitizen = "^3.2.2"
 doc8 = "^0.10.1"
 flake8 = "^6.0.0"
 isort = "^5.11.4"
 mypy = "^0.991"
 sphinx-rtd-theme = "^1.1.1"
 types-docutils = "^0.19.1.2"
 
@@ -81,15 +81,15 @@
 logbook = "^1.5.3"
 pyqt5 = "^5.15.7"
 pyqtgraph = "^0.13.1"
 spyder = "^5.4.1"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.0"
+version = "0.6.0"
 major_version_zero = true
 tag_format = "$version"
 annotated_tag = true
 version_files = [
     "pyproject.toml",
     "sphinxcontrib/cadquery/__init__.py",
 ]
```

### Comparing `sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/__init__.py` & `sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .cq_core import (
     CqSvgDirective,
     CqVtkDirective,
     LegacyCqSvgDirective,
     LegacyCqVtkDirective,
 )
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 _ROOT_DIR = Path(__file__).absolute().parent
 
 _JS_FILES = {
     "static/dist/vtk-lite.js": {"priority": 90},
     "static/render.js": {"priority": 100},
 }
```

### Comparing `sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/cq_core.py` & `sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/cq_core.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/static/cadquery.css` & `sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/static/cadquery.css`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 }
 
 .cadquery-align-center {
     margin: 0px auto;
 }
 
 .cadquery-container-model {
+    border: 1px solid #ddd;
     color: white;
     position: relative;
 }
 
 button.cadquery-credit {
     border: 1px;
     color: white;
```

### Comparing `sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/static/dist/vtk-lite.js` & `sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/static/dist/vtk-lite.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/static/render.js` & `sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/static/render.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/templates/svg.rst.jinja` & `sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/templates/svg.rst.jinja`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_cadquery-0.5.0/sphinxcontrib/cadquery/templates/vtk.rst.jinja` & `sphinxcontrib_cadquery-0.6.0/sphinxcontrib/cadquery/templates/vtk.rst.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. raw:: html
 
     <div class="cadquery-container cadquery-align-{{align}}" style="margin-bottom: 24px; width:{{width}};">
         <div class="cadquery-container-model">
-            <div class="cadquery-vtk" style="height:{{height}};border: 1px solid #ddd;">
+            <div class="cadquery-vtk" style="height:{{height}};">
                 <script>
                     var parent_element = {{element}};
                     var data = {{vtk_json}};
                     render(data, parent_element);
                 </script>
             </div>
             <div class="cadquery-help-dropdown">
```

### Comparing `sphinxcontrib_cadquery-0.5.0/PKG-INFO` & `sphinxcontrib_cadquery-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-cadquery
-Version: 0.5.0
+Version: 0.6.0
 Summary: Sphinx extension for rendering CadQuery models.
 Home-page: https://github.com/sethfischer/sphinxcontrib-cadquery
 License: Apache-2.0
 Keywords: cad,cadquery,parametric,programmatic,sphinx,svg,vtk,vtk.js
 Author: Seth Fischer
 Author-email: seth@fischer.nz
 Requires-Python: >=3.9,<3.11
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: Sphinx (>=5.3.0,<6.0.0)
+Requires-Dist: Sphinx (>=5.3.0,<7.0.0)
 Requires-Dist: ipython (>=7.31.1)
 Requires-Dist: jinja2 (>=3.0)
 Project-URL: Bug Tracker, https://github.com/sethfischer/sphinxcontrib-cadquery/issues
 Project-URL: Documentation, https://sphinxcontrib-cadquery.readthedocs.io/
 Project-URL: Repository, https://github.com/sethfischer/sphinxcontrib-cadquery.git
 Description-Content-Type: text/x-rst
```

