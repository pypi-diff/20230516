# Comparing `tmp/petab-0.2.0.tar.gz` & `tmp/petab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petab-0.2.0.tar", last modified: Mon May  8 15:43:50 2023, max compression
+gzip compressed data, was "petab-0.2.1.tar", last modified: Tue May 16 13:17:02 2023, max compression
```

## Comparing `petab-0.2.0.tar` & `petab-0.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-08 15:43:41.000000 petab-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 15:43:41.000000 petab-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-08 15:43:50.778574 petab-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-08 15:43:41.000000 petab-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-08 15:43:41.000000 petab-0.2.0/petab/C.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-08 15:43:41.000000 petab-0.2.0/petab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-08 15:43:41.000000 petab-0.2.0/petab/calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-08 15:43:41.000000 petab-0.2.0/petab/composite_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-08 15:43:41.000000 petab-0.2.0/petab/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-05-08 15:43:41.000000 petab-0.2.0/petab/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 15:43:41.000000 petab-0.2.0/petab/format_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    38465 2023-05-08 15:43:41.000000 petab-0.2.0/petab/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-08 15:43:41.000000 petab-0.2.0/petab/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-05-08 15:43:41.000000 petab-0.2.0/petab/measurements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/models/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-08 15:43:41.000000 petab-0.2.0/petab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-08 15:43:41.000000 petab-0.2.0/petab/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-08 15:43:41.000000 petab-0.2.0/petab/models/pysb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-08 15:43:41.000000 petab-0.2.0/petab/models/sbml_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-08 15:43:41.000000 petab-0.2.0/petab/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-05-08 15:43:41.000000 petab-0.2.0/petab/parameter_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-05-08 15:43:41.000000 petab-0.2.0/petab/parameters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4855 2023-05-08 15:43:41.000000 petab-0.2.0/petab/petablint.py
--rw-r--r--   0 runner    (1001) docker     (123)    33069 2023-05-08 15:43:41.000000 petab-0.2.0/petab/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-08 15:43:41.000000 petab-0.2.0/petab/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-08 15:43:41.000000 petab-0.2.0/petab/sbml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-08 15:43:41.000000 petab-0.2.0/petab/schemas/petab_schema.v1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-08 15:43:41.000000 petab-0.2.0/petab/schemas/petab_schema.v2.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-08 15:43:41.000000 petab-0.2.0/petab/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-08 15:43:41.000000 petab-0.2.0/petab/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 15:43:41.000000 petab-0.2.0/petab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/data_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/plot_data_and_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/plot_residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab/visualize/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/templates/mystyle.css
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 15:43:41.000000 petab-0.2.0/petab/visualize/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-05-08 15:43:41.000000 petab-0.2.0/petab/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:43:50.778574 petab-0.2.0/petab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 15:43:50.000000 petab-0.2.0/petab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 15:43:41.000000 petab-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:43:50.778574 petab-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-08 15:43:41.000000 petab-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.761197 petab-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 13:16:49.000000 petab-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 13:16:49.000000 petab-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-16 13:17:02.761197 petab-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-16 13:16:49.000000 petab-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.749197 petab-0.2.1/petab/
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-16 13:16:50.000000 petab-0.2.1/petab/C.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-16 13:16:50.000000 petab-0.2.1/petab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-16 13:16:50.000000 petab-0.2.1/petab/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-16 13:16:50.000000 petab-0.2.1/petab/composite_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-16 13:16:50.000000 petab-0.2.1/petab/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-05-16 13:16:50.000000 petab-0.2.1/petab/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:16:50.000000 petab-0.2.1/petab/format_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38465 2023-05-16 13:16:50.000000 petab-0.2.1/petab/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-16 13:16:50.000000 petab-0.2.1/petab/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-05-16 13:16:50.000000 petab-0.2.1/petab/measurements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.757197 petab-0.2.1/petab/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 13:16:50.000000 petab-0.2.1/petab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-16 13:16:50.000000 petab-0.2.1/petab/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-05-16 13:16:50.000000 petab-0.2.1/petab/models/pysb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-16 13:16:50.000000 petab-0.2.1/petab/models/sbml_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-16 13:16:50.000000 petab-0.2.1/petab/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-05-16 13:16:50.000000 petab-0.2.1/petab/parameter_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-05-16 13:16:50.000000 petab-0.2.1/petab/parameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4855 2023-05-16 13:16:50.000000 petab-0.2.1/petab/petablint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-05-16 13:16:50.000000 petab-0.2.1/petab/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-16 13:16:50.000000 petab-0.2.1/petab/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-16 13:16:50.000000 petab-0.2.1/petab/sbml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.757197 petab-0.2.1/petab/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-16 13:16:50.000000 petab-0.2.1/petab/schemas/petab_schema.v1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-16 13:16:50.000000 petab-0.2.1/petab/schemas/petab_schema.v2.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-16 13:16:50.000000 petab-0.2.1/petab/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-16 13:16:50.000000 petab-0.2.1/petab/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 13:16:50.000000 petab-0.2.1/petab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.761197 petab-0.2.1/petab/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/data_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/plot_data_and_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/plot_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.761197 petab-0.2.1/petab/visualize/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/templates/mystyle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-05-16 13:16:50.000000 petab-0.2.1/petab/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.757197 petab-0.2.1/petab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 13:16:50.000000 petab-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:17:02.761197 petab-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-16 13:16:50.000000 petab-0.2.1/setup.py
```

### Comparing `petab-0.2.0/LICENSE` & `petab-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/PKG-INFO` & `petab-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parameter estimation tabular data
 Home-page: https://github.com/PEtab-dev/libpetab-python
 Author: The PEtab developers
 Author-email: daniel.weindl@helmholtz-muenchen.de
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: tests
@@ -35,15 +35,15 @@
 ## Installation
 
 The PEtab library is available on [pypi](https://pypi.org/project/petab/)
 and the easiest way to install it is running
 
     pip3 install petab
     
-It will require Python>=3.8 to run. (We are following the
+It will require Python>=3.9 to run. (We are following the
 [numpy Python support policy](https://numpy.org/neps/nep-0029-deprecation_policy.html)).
 
 Development versions of the PEtab library can be installed using
 
     pip3 install https://github.com/PEtab-dev/libpetab-python/archive/develop.zip
 
 (replace `develop` by the branch or commit you would like to install).
```

### Comparing `petab-0.2.0/README.md` & `petab-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ## Installation
 
 The PEtab library is available on [pypi](https://pypi.org/project/petab/)
 and the easiest way to install it is running
 
     pip3 install petab
     
-It will require Python>=3.8 to run. (We are following the
+It will require Python>=3.9 to run. (We are following the
 [numpy Python support policy](https://numpy.org/neps/nep-0029-deprecation_policy.html)).
 
 Development versions of the PEtab library can be installed using
 
     pip3 install https://github.com/PEtab-dev/libpetab-python/archive/develop.zip
 
 (replace `develop` by the branch or commit you would like to install).
```

### Comparing `petab-0.2.0/petab/C.py` & `petab-0.2.1/petab/C.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/__init__.py` & `petab-0.2.1/petab/__init__.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/calculate.py` & `petab-0.2.1/petab/calculate.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/composite_problem.py` & `petab-0.2.1/petab/composite_problem.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/conditions.py` & `petab-0.2.1/petab/conditions.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/core.py` & `petab-0.2.1/petab/core.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/lint.py` & `petab-0.2.1/petab/lint.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/mapping.py` & `petab-0.2.1/petab/mapping.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/measurements.py` & `petab-0.2.1/petab/measurements.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/models/model.py` & `petab-0.2.1/petab/models/model.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/models/pysb_model.py` & `petab-0.2.1/petab/models/pysb_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self._model_id = model_id
 
     def get_parameter_ids(self) -> Iterable[str]:
         return (p.name for p in self.model.parameters)
 
     def get_parameter_value(self, id_: str) -> float:
         try:
-            return self.model.parameters[id_].name
+            return self.model.parameters[id_].value
         except KeyError as e:
             raise ValueError(f"Parameter {id_} does not exist.") from e
 
     def get_free_parameter_ids_with_values(
             self
     ) -> Iterable[Tuple[str, float]]:
         return ((p.name, p.value) for p in self.model.parameters)
```

### Comparing `petab-0.2.0/petab/models/sbml_model.py` & `petab-0.2.1/petab/models/sbml_model.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/observables.py` & `petab-0.2.1/petab/observables.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/parameter_mapping.py` & `petab-0.2.1/petab/parameter_mapping.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/parameters.py` & `petab-0.2.1/petab/parameters.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/petablint.py` & `petab-0.2.1/petab/petablint.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/problem.py` & `petab-0.2.1/petab/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,15 +407,15 @@
             if getattr(self, f'{table_name}_df') is not None:
                 filenames[f'{table_name}_file'] = f'{table_name}s.tsv'
 
         if self.model:
             if not isinstance(self.model, SbmlModel):
                 raise NotImplementedError("Saving non-SBML models is "
                                           "currently not supported.")
-            filenames['sbml_file'] = 'model.xml'
+            filenames['model_file'] = 'model.xml'
 
         filenames['yaml_file'] = 'problem.yaml'
 
         self.to_files(**filenames, prefix_path=prefix_path)
 
         if prefix_path is None:
             return filenames['yaml_file']
@@ -538,15 +538,15 @@
             if self.mapping_df is not None:
                 mapping.write_mapping_df(self.mapping_df, mapping_file)
             else:
                 raise error("mapping")
 
         if yaml_file:
             yaml.create_problem_yaml(
-                sbml_files=sbml_file,
+                sbml_files=model_file,
                 condition_files=condition_file,
                 measurement_files=measurement_file,
                 parameter_file=parameter_file,
                 observable_files=observable_file,
                 yaml_file=yaml_file,
                 visualization_files=visualization_file,
                 relative_paths=relative_paths,
```

### Comparing `petab-0.2.0/petab/sampling.py` & `petab-0.2.1/petab/sampling.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/sbml.py` & `petab-0.2.1/petab/sbml.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/schemas/petab_schema.v1.0.0.yaml` & `petab-0.2.1/petab/schemas/petab_schema.v1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/schemas/petab_schema.v2.0.0.yaml` & `petab-0.2.1/petab/schemas/petab_schema.v2.0.0.yaml`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/simplify.py` & `petab-0.2.1/petab/simplify.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/simulate.py` & `petab-0.2.1/petab/simulate.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/__init__.py` & `petab-0.2.1/petab/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/cli.py` & `petab-0.2.1/petab/visualize/cli.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/data_overview.py` & `petab-0.2.1/petab/visualize/data_overview.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/helper_functions.py` & `petab-0.2.1/petab/visualize/helper_functions.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/lint.py` & `petab-0.2.1/petab/visualize/lint.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/plot_data_and_simulation.py` & `petab-0.2.1/petab/visualize/plot_data_and_simulation.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/plot_residuals.py` & `petab-0.2.1/petab/visualize/plot_residuals.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/plotter.py` & `petab-0.2.1/petab/visualize/plotter.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/plotting.py` & `petab-0.2.1/petab/visualize/plotting.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/visualize/templates/report.html` & `petab-0.2.1/petab/visualize/templates/report.html`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab/yaml.py` & `petab-0.2.1/petab/yaml.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/petab.egg-info/PKG-INFO` & `petab-0.2.1/petab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parameter estimation tabular data
 Home-page: https://github.com/PEtab-dev/libpetab-python
 Author: The PEtab developers
 Author-email: daniel.weindl@helmholtz-muenchen.de
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: tests
@@ -35,15 +35,15 @@
 ## Installation
 
 The PEtab library is available on [pypi](https://pypi.org/project/petab/)
 and the easiest way to install it is running
 
     pip3 install petab
     
-It will require Python>=3.8 to run. (We are following the
+It will require Python>=3.9 to run. (We are following the
 [numpy Python support policy](https://numpy.org/neps/nep-0029-deprecation_policy.html)).
 
 Development versions of the PEtab library can be installed using
 
     pip3 install https://github.com/PEtab-dev/libpetab-python/archive/develop.zip
 
 (replace `develop` by the branch or commit you would like to install).
```

### Comparing `petab-0.2.0/petab.egg-info/SOURCES.txt` & `petab-0.2.1/petab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petab-0.2.0/setup.py` & `petab-0.2.1/setup.py`

 * *Files identical despite different names*

