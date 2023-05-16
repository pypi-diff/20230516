# Comparing `tmp/corrct-0.8.0.tar.gz` & `tmp/corrct-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corrct-0.8.0.tar", last modified: Thu Apr  6 18:04:36 2023, max compression
+gzip compressed data, was "corrct-0.8.1.tar", last modified: Tue May 16 14:01:03 2023, max compression
```

## Comparing `corrct-0.8.0.tar` & `corrct-0.8.1.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxr-xr-x   0 vigano    (1000) users      (100)        0 2023-04-06 18:04:36.434617 corrct-0.8.0/
--rwxr-xr-x   0 vigano    (1000) users      (100)     9534 2023-04-06 17:26:44.000000 corrct-0.8.0/CHANGELOG.md
--rw-r--r--   0 vigano    (1000) users      (100)     1515 2022-09-15 17:06:44.000000 corrct-0.8.0/LICENSE.md
--rw-r--r--   0 vigano    (1000) users      (100)       22 2022-09-15 17:06:44.000000 corrct-0.8.0/MANIFEST.in
--rw-r--r--   0 vigano    (1000) users      (100)    14347 2023-04-06 18:04:36.434617 corrct-0.8.0/PKG-INFO
--rwxr-xr-x   0 vigano    (1000) users      (100)     3944 2022-10-28 09:49:00.000000 corrct-0.8.0/README.md
-drwxr-xr-x   0 vigano    (1000) users      (100)        0 2023-04-06 18:04:36.434617 corrct-0.8.0/corrct/
--rwxr-xr-x   0 vigano    (1000) users      (100)        5 2023-04-06 16:21:27.000000 corrct-0.8.0/corrct/VERSION
--rw-r--r--   0 vigano    (1000) users      (100)     1297 2023-04-06 15:56:41.000000 corrct-0.8.0/corrct/__init__.py
--rwxr-xr-x   0 vigano    (1000) users      (100)     6386 2022-10-28 09:49:00.000000 corrct-0.8.0/corrct/_corrct.py
--rw-r--r--   0 vigano    (1000) users      (100)    26095 2022-12-08 14:30:27.000000 corrct-0.8.0/corrct/_projector_backends.py
--rw-r--r--   0 vigano    (1000) users      (100)    10415 2023-02-16 15:32:25.000000 corrct-0.8.0/corrct/attenuation.py
--rw-r--r--   0 vigano    (1000) users      (100)    19437 2023-04-06 13:12:03.000000 corrct-0.8.0/corrct/data_terms.py
--rw-r--r--   0 vigano    (1000) users      (100)     3825 2023-02-28 13:39:27.000000 corrct-0.8.0/corrct/denoisers.py
--rw-r--r--   0 vigano    (1000) users      (100)    19249 2023-02-28 13:39:27.000000 corrct-0.8.0/corrct/filters.py
--rw-r--r--   0 vigano    (1000) users      (100)    12338 2023-04-06 16:04:37.000000 corrct-0.8.0/corrct/models.py
--rwxr-xr-x   0 vigano    (1000) users      (100)    30716 2022-11-09 14:22:27.000000 corrct-0.8.0/corrct/operators.py
--rw-r--r--   0 vigano    (1000) users      (100)    21272 2023-02-16 15:32:25.000000 corrct-0.8.0/corrct/param_tuning.py
--rw-r--r--   0 vigano    (1000) users      (100)    20668 2023-02-16 15:32:25.000000 corrct-0.8.0/corrct/physics.py
--rwxr-xr-x   0 vigano    (1000) users      (100)    24225 2023-04-06 13:12:23.000000 corrct-0.8.0/corrct/projectors.py
--rw-r--r--   0 vigano    (1000) users      (100)    45381 2023-02-16 15:32:25.000000 corrct-0.8.0/corrct/regularizers.py
--rw-r--r--   0 vigano    (1000) users      (100)    35110 2022-12-08 14:30:27.000000 corrct-0.8.0/corrct/solvers.py
--rw-r--r--   0 vigano    (1000) users      (100)    23094 2023-02-28 13:31:26.000000 corrct-0.8.0/corrct/struct_illum.py
--rw-r--r--   0 vigano    (1000) users      (100)    16010 2023-02-28 13:39:27.000000 corrct-0.8.0/corrct/testing.py
-drwxr-xr-x   0 vigano    (1000) users      (100)        0 2023-04-06 18:04:36.434617 corrct-0.8.0/corrct.egg-info/
--rw-r--r--   0 vigano    (1000) users      (100)    14347 2023-04-06 18:04:36.000000 corrct-0.8.0/corrct.egg-info/PKG-INFO
--rw-r--r--   0 vigano    (1000) users      (100)      722 2023-04-06 18:04:36.000000 corrct-0.8.0/corrct.egg-info/SOURCES.txt
--rw-r--r--   0 vigano    (1000) users      (100)        1 2023-04-06 18:04:36.000000 corrct-0.8.0/corrct.egg-info/dependency_links.txt
--rw-r--r--   0 vigano    (1000) users      (100)        1 2022-09-15 17:06:44.000000 corrct-0.8.0/corrct.egg-info/not-zip-safe
--rw-r--r--   0 vigano    (1000) users      (100)       89 2023-04-06 18:04:36.000000 corrct-0.8.0/corrct.egg-info/requires.txt
--rw-r--r--   0 vigano    (1000) users      (100)        7 2023-04-06 18:04:36.000000 corrct-0.8.0/corrct.egg-info/top_level.txt
--rw-r--r--   0 vigano    (1000) users      (100)       89 2022-09-15 17:06:44.000000 corrct-0.8.0/pyproject.toml
--rw-r--r--   0 vigano    (1000) users      (100)     1142 2023-04-06 18:04:36.434617 corrct-0.8.0/setup.cfg
--rw-r--r--   0 vigano    (1000) users      (100)      141 2022-09-15 17:06:44.000000 corrct-0.8.0/setup.py
-drwxr-xr-x   0 vigano    (1000) users      (100)        0 2023-04-06 18:04:36.434617 corrct-0.8.0/tests/
--rw-r--r--   0 vigano    (1000) users      (100)      639 2022-09-15 17:06:44.000000 corrct-0.8.0/tests/test_examples.py
--rwxr-xr-x   0 vigano    (1000) users      (100)     9635 2022-10-28 09:49:00.000000 corrct-0.8.0/tests/test_operators.py
--rw-r--r--   0 vigano    (1000) users      (100)     3939 2022-10-28 09:49:00.000000 corrct-0.8.0/tests/test_projectors.py
--rw-r--r--   0 vigano    (1000) users      (100)     5074 2023-02-16 15:29:22.000000 corrct-0.8.0/tests/test_regularizers.py
--rwxr-xr-x   0 vigano    (1000) users      (100)     6346 2022-10-28 09:49:00.000000 corrct-0.8.0/tests/test_solvers.py
+drwxr-xr-x   0 vigano    (1000) users      (100)        0 2023-05-16 14:01:03.332093 corrct-0.8.1/
+-rwxr-xr-x   0 vigano    (1000) users      (100)     9641 2023-05-16 13:54:47.000000 corrct-0.8.1/CHANGELOG.md
+-rw-r--r--   0 vigano    (1000) users      (100)     1515 2022-09-15 17:06:44.000000 corrct-0.8.1/LICENSE.md
+-rw-r--r--   0 vigano    (1000) users      (100)       22 2022-09-15 17:06:44.000000 corrct-0.8.1/MANIFEST.in
+-rw-r--r--   0 vigano    (1000) users      (100)    14454 2023-05-16 14:01:03.332093 corrct-0.8.1/PKG-INFO
+-rwxr-xr-x   0 vigano    (1000) users      (100)     3944 2022-10-28 09:49:00.000000 corrct-0.8.1/README.md
+drwxr-xr-x   0 vigano    (1000) users      (100)        0 2023-05-16 14:01:03.328093 corrct-0.8.1/corrct/
+-rwxr-xr-x   0 vigano    (1000) users      (100)        5 2023-05-16 13:52:50.000000 corrct-0.8.1/corrct/VERSION
+-rw-r--r--   0 vigano    (1000) users      (100)     1297 2023-05-16 11:54:43.000000 corrct-0.8.1/corrct/__init__.py
+-rwxr-xr-x   0 vigano    (1000) users      (100)     6386 2022-10-28 09:49:00.000000 corrct-0.8.1/corrct/_corrct.py
+-rw-r--r--   0 vigano    (1000) users      (100)    26095 2022-12-08 14:30:27.000000 corrct-0.8.1/corrct/_projector_backends.py
+-rw-r--r--   0 vigano    (1000) users      (100)    10415 2023-02-16 15:32:25.000000 corrct-0.8.1/corrct/attenuation.py
+-rw-r--r--   0 vigano    (1000) users      (100)    19437 2023-04-06 13:12:03.000000 corrct-0.8.1/corrct/data_terms.py
+-rw-r--r--   0 vigano    (1000) users      (100)     3825 2023-02-28 13:39:27.000000 corrct-0.8.1/corrct/denoisers.py
+-rw-r--r--   0 vigano    (1000) users      (100)    19249 2023-02-28 13:39:27.000000 corrct-0.8.1/corrct/filters.py
+-rw-r--r--   0 vigano    (1000) users      (100)    12338 2023-04-06 20:03:16.000000 corrct-0.8.1/corrct/models.py
+-rwxr-xr-x   0 vigano    (1000) users      (100)    30716 2022-11-09 14:22:27.000000 corrct-0.8.1/corrct/operators.py
+-rw-r--r--   0 vigano    (1000) users      (100)    21272 2023-02-16 15:32:25.000000 corrct-0.8.1/corrct/param_tuning.py
+-rw-r--r--   0 vigano    (1000) users      (100)    20668 2023-02-16 15:32:25.000000 corrct-0.8.1/corrct/physics.py
+drwxr-xr-x   0 vigano    (1000) users      (100)        0 2023-05-16 14:01:03.332093 corrct-0.8.1/corrct/processing/
+-rw-r--r--   0 vigano    (1000) users      (100)      662 2022-10-28 09:49:00.000000 corrct-0.8.1/corrct/processing/__init__.py
+-rw-r--r--   0 vigano    (1000) users      (100)    17396 2023-05-16 10:13:42.000000 corrct-0.8.1/corrct/processing/misc.py
+-rw-r--r--   0 vigano    (1000) users      (100)     4540 2023-04-06 13:12:16.000000 corrct-0.8.1/corrct/processing/noise.py
+-rw-r--r--   0 vigano    (1000) users      (100)    11576 2023-05-16 10:13:42.000000 corrct-0.8.1/corrct/processing/post.py
+-rw-r--r--   0 vigano    (1000) users      (100)     6704 2023-05-16 11:54:43.000000 corrct-0.8.1/corrct/processing/pre.py
+-rwxr-xr-x   0 vigano    (1000) users      (100)    24225 2023-04-06 13:12:23.000000 corrct-0.8.1/corrct/projectors.py
+-rw-r--r--   0 vigano    (1000) users      (100)    45381 2023-02-16 15:32:25.000000 corrct-0.8.1/corrct/regularizers.py
+-rw-r--r--   0 vigano    (1000) users      (100)    35110 2022-12-08 14:30:27.000000 corrct-0.8.1/corrct/solvers.py
+-rw-r--r--   0 vigano    (1000) users      (100)    23094 2023-02-28 13:31:26.000000 corrct-0.8.1/corrct/struct_illum.py
+-rw-r--r--   0 vigano    (1000) users      (100)    16010 2023-02-28 13:39:27.000000 corrct-0.8.1/corrct/testing.py
+drwxr-xr-x   0 vigano    (1000) users      (100)        0 2023-05-16 14:01:03.332093 corrct-0.8.1/corrct.egg-info/
+-rw-r--r--   0 vigano    (1000) users      (100)    14454 2023-05-16 14:01:03.000000 corrct-0.8.1/corrct.egg-info/PKG-INFO
+-rw-r--r--   0 vigano    (1000) users      (100)      856 2023-05-16 14:01:03.000000 corrct-0.8.1/corrct.egg-info/SOURCES.txt
+-rw-r--r--   0 vigano    (1000) users      (100)        1 2023-05-16 14:01:03.000000 corrct-0.8.1/corrct.egg-info/dependency_links.txt
+-rw-r--r--   0 vigano    (1000) users      (100)        1 2022-09-15 17:06:44.000000 corrct-0.8.1/corrct.egg-info/not-zip-safe
+-rw-r--r--   0 vigano    (1000) users      (100)       89 2023-05-16 14:01:03.000000 corrct-0.8.1/corrct.egg-info/requires.txt
+-rw-r--r--   0 vigano    (1000) users      (100)        7 2023-05-16 14:01:03.000000 corrct-0.8.1/corrct.egg-info/top_level.txt
+-rw-r--r--   0 vigano    (1000) users      (100)       89 2022-09-15 17:06:44.000000 corrct-0.8.1/pyproject.toml
+-rw-r--r--   0 vigano    (1000) users      (100)     1195 2023-05-16 14:01:03.332093 corrct-0.8.1/setup.cfg
+-rw-r--r--   0 vigano    (1000) users      (100)      141 2023-05-16 13:50:39.000000 corrct-0.8.1/setup.py
+drwxr-xr-x   0 vigano    (1000) users      (100)        0 2023-05-16 14:01:03.332093 corrct-0.8.1/tests/
+-rw-r--r--   0 vigano    (1000) users      (100)      639 2022-09-15 17:06:44.000000 corrct-0.8.1/tests/test_examples.py
+-rwxr-xr-x   0 vigano    (1000) users      (100)     9635 2022-10-28 09:49:00.000000 corrct-0.8.1/tests/test_operators.py
+-rw-r--r--   0 vigano    (1000) users      (100)     3939 2022-10-28 09:49:00.000000 corrct-0.8.1/tests/test_projectors.py
+-rw-r--r--   0 vigano    (1000) users      (100)     5074 2023-02-16 15:29:22.000000 corrct-0.8.1/tests/test_regularizers.py
+-rwxr-xr-x   0 vigano    (1000) users      (100)     6346 2022-10-28 09:49:00.000000 corrct-0.8.1/tests/test_solvers.py
```

### Comparing `corrct-0.8.0/CHANGELOG.md` & `corrct-0.8.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-[Unreleased]: https://www.github.com/cicwi/corrct/compare/v0.8.0...develop
+[Unreleased]: https://www.github.com/cicwi/corrct/compare/v0.8.1...develop
+
+## 0.8.1 - 2023-05-16
+### Added
+- Power spectrum calculation function.
+### Fixed
+- Pypi package creation.
 
 ## 0.8.0 - 2023-04-06
 ### Added
 - Ghost imaging support (structured illumination):
   - Theoretical mask generation (incl. MURA, Half-Gaussian, Bernoulli)
   - Dedicated projector (CPU based).
 ### Fixed
```

### Comparing `corrct-0.8.0/LICENSE.md` & `corrct-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/PKG-INFO` & `corrct-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corrct
-Version: 0.8.0
+Version: 0.8.1
 Summary: Physically corrected projectors for X-ray induced emission CT.
 Home-page: https://github.com/cicwi/PyCorrectedEmissionCT
 Author: Nicola VIGANÒ
 Author-email: N.R.Vigano@cwi.nl
 License: BSD license
 Keywords: corrct,xrf-ct,xrd-ct,self-attenuation,attenuation correction
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -125,15 +125,21 @@
 
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-[Unreleased]: https://www.github.com/cicwi/corrct/compare/v0.8.0...develop
+[Unreleased]: https://www.github.com/cicwi/corrct/compare/v0.8.1...develop
+
+## 0.8.1 - 2023-05-16
+### Added
+- Power spectrum calculation function.
+### Fixed
+- Pypi package creation.
 
 ## 0.8.0 - 2023-04-06
 ### Added
 - Ghost imaging support (structured illumination):
   - Theoretical mask generation (incl. MURA, Half-Gaussian, Bernoulli)
   - Dedicated projector (CPU based).
 ### Fixed
```

### Comparing `corrct-0.8.0/README.md` & `corrct-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/__init__.py` & `corrct-0.8.1/corrct/__init__.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/_corrct.py` & `corrct-0.8.1/corrct/_corrct.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/_projector_backends.py` & `corrct-0.8.1/corrct/_projector_backends.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/attenuation.py` & `corrct-0.8.1/corrct/attenuation.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/data_terms.py` & `corrct-0.8.1/corrct/data_terms.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/denoisers.py` & `corrct-0.8.1/corrct/denoisers.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/filters.py` & `corrct-0.8.1/corrct/filters.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/models.py` & `corrct-0.8.1/corrct/models.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/operators.py` & `corrct-0.8.1/corrct/operators.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/param_tuning.py` & `corrct-0.8.1/corrct/param_tuning.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/physics.py` & `corrct-0.8.1/corrct/physics.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/projectors.py` & `corrct-0.8.1/corrct/projectors.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/regularizers.py` & `corrct-0.8.1/corrct/regularizers.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/solvers.py` & `corrct-0.8.1/corrct/solvers.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/struct_illum.py` & `corrct-0.8.1/corrct/struct_illum.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct/testing.py` & `corrct-0.8.1/corrct/testing.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/corrct.egg-info/PKG-INFO` & `corrct-0.8.1/corrct.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corrct
-Version: 0.8.0
+Version: 0.8.1
 Summary: Physically corrected projectors for X-ray induced emission CT.
 Home-page: https://github.com/cicwi/PyCorrectedEmissionCT
 Author: Nicola VIGANÒ
 Author-email: N.R.Vigano@cwi.nl
 License: BSD license
 Keywords: corrct,xrf-ct,xrd-ct,self-attenuation,attenuation correction
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -125,15 +125,21 @@
 
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-[Unreleased]: https://www.github.com/cicwi/corrct/compare/v0.8.0...develop
+[Unreleased]: https://www.github.com/cicwi/corrct/compare/v0.8.1...develop
+
+## 0.8.1 - 2023-05-16
+### Added
+- Power spectrum calculation function.
+### Fixed
+- Pypi package creation.
 
 ## 0.8.0 - 2023-04-06
 ### Added
 - Ghost imaging support (structured illumination):
   - Theoretical mask generation (incl. MURA, Half-Gaussian, Bernoulli)
   - Dedicated projector (CPU based).
 ### Fixed
```

### Comparing `corrct-0.8.0/corrct.egg-info/SOURCES.txt` & `corrct-0.8.1/corrct.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -24,12 +24,17 @@
 corrct/testing.py
 corrct.egg-info/PKG-INFO
 corrct.egg-info/SOURCES.txt
 corrct.egg-info/dependency_links.txt
 corrct.egg-info/not-zip-safe
 corrct.egg-info/requires.txt
 corrct.egg-info/top_level.txt
+corrct/processing/__init__.py
+corrct/processing/misc.py
+corrct/processing/noise.py
+corrct/processing/post.py
+corrct/processing/pre.py
 tests/test_examples.py
 tests/test_operators.py
 tests/test_projectors.py
 tests/test_regularizers.py
 tests/test_solvers.py
```

### Comparing `corrct-0.8.0/setup.cfg` & `corrct-0.8.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -19,24 +19,29 @@
 license = BSD license
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = False
 include_package_data = True
-packages = corrct
+packages = find:
 python_requires = >=3.7
 install_requires = 
 	numpy>=1.21
 	scipy
 	tqdm
 	scikit-image
 	PyWavelets
 	matplotlib
 
+[options.packages.find]
+include = 
+	corrct
+	corrct.*
+
 [options.extras_require]
 dev = 
 	sphinx
 	sphinx_rtd_theme
 
 [bdist_wheel]
 universal = 0
```

### Comparing `corrct-0.8.0/tests/test_examples.py` & `corrct-0.8.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/tests/test_operators.py` & `corrct-0.8.1/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/tests/test_projectors.py` & `corrct-0.8.1/tests/test_projectors.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/tests/test_regularizers.py` & `corrct-0.8.1/tests/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `corrct-0.8.0/tests/test_solvers.py` & `corrct-0.8.1/tests/test_solvers.py`

 * *Files identical despite different names*

