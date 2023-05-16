# Comparing `tmp/openpile-0.3.0.tar.gz` & `tmp/openpile-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-72ls0hyh/openpile-0.3.0.tar", last modified: Tue May  2 19:18:08 2023, max compression
+gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-8svl9kor/openpile-0.3.1.tar", last modified: Tue May 16 18:48:55 2023, max compression
```

## Comparing `openpile-0.3.0.tar` & `openpile-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 19:17:55.000000 openpile-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-02 19:18:08.000000 openpile-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-02 19:17:55.000000 openpile-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-02 19:17:55.000000 openpile-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-02 19:18:08.000000 openpile-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-02 19:17:55.000000 openpile-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)    54305 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/soilmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/Hb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/Mb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/mt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/py_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/qz_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-02 19:17:55.000000 openpile-0.3.0/src/openpile/utils/tz_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 19:18:08.000000 openpile-0.3.0/src/openpile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:18:08.000000 openpile-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-02 19:17:55.000000 openpile-0.3.0/test/test_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-02 19:17:55.000000 openpile-0.3.0/test/test_pycurves.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-02 19:17:55.000000 openpile-0.3.0/test/test_utils_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 18:48:46.000000 openpile-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-16 18:48:55.000000 openpile-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-16 18:48:46.000000 openpile-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 18:48:46.000000 openpile-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-16 18:48:55.000000 openpile-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-16 18:48:46.000000 openpile-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54305 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/soilmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/Hb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/Mb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/mt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/py_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/qz_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-16 18:48:46.000000 openpile-0.3.1/src/openpile/utils/tz_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 18:48:55.000000 openpile-0.3.1/src/openpile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:48:55.000000 openpile-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-16 18:48:46.000000 openpile-0.3.1/test/test_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-16 18:48:46.000000 openpile-0.3.1/test/test_pycurves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-16 18:48:46.000000 openpile-0.3.1/test/test_utils_misc.py
```

### Comparing `openpile-0.3.0/LICENSE.txt` & `openpile-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/PKG-INFO` & `openpile-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
```

### Comparing `openpile-0.3.0/README.md` & `openpile-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/setup.cfg` & `openpile-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 python_requires = >=3.7
 install_requires = 
 	pandas
 	numpy
 	matplotlib
 	numba
 	scipy
-	fpdf2
 	pydantic
 	typing_extensions
 
 [options.extras_require]
 dev = 
 	Sphinx==5.3.0
 	sphinx-rtd-theme==1.1.1
```

### Comparing `openpile-0.3.0/setup.py` & `openpile-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/analyses.py` & `openpile-0.3.1/src/openpile/analyses.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/construct.py` & `openpile-0.3.1/src/openpile/construct.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/core/kernel.py` & `openpile-0.3.1/src/openpile/core/kernel.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/core/misc.py` & `openpile-0.3.1/src/openpile/core/misc.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/core/txt.py` & `openpile-0.3.1/src/openpile/core/txt.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/core/validation.py` & `openpile-0.3.1/src/openpile/core/validation.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/soilmodels.py` & `openpile-0.3.1/src/openpile/soilmodels.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/utils/Hb_curves.py` & `openpile-0.3.1/src/openpile/utils/Hb_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/utils/Mb_curves.py` & `openpile-0.3.1/src/openpile/utils/Mb_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/utils/graphics.py` & `openpile-0.3.1/src/openpile/utils/graphics.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/utils/mt_curves.py` & `openpile-0.3.1/src/openpile/utils/mt_curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     m_max = m_m1 + m_m2 * X / D
     psi_max = m_max / k
 
     # calculate normsalised conic function
     t, m = conic(psi_max, n, k, m_max, output_length)
 
     # return non-normalised curve
-    return m * (Su * D**2), t * (Su / G0)
+    return m * (Su * D), t * (Su / G0)
 
 
 @njit(cache=True)
 def dunkirk_sand(
     sig: float,
     X: float,
     Dr: float,
```

### Comparing `openpile-0.3.0/src/openpile/utils/py_curves.py` & `openpile-0.3.1/src/openpile/utils/py_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/utils/qz_curves.py` & `openpile-0.3.1/src/openpile/utils/qz_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile/utils/tz_curves.py` & `openpile-0.3.1/src/openpile/utils/tz_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/src/openpile.egg-info/PKG-INFO` & `openpile-0.3.1/src/openpile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
 Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/TchilDill/openpile
```

### Comparing `openpile-0.3.0/src/openpile.egg-info/SOURCES.txt` & `openpile-0.3.1/src/openpile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/test/test_construct.py` & `openpile-0.3.1/test/test_construct.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/test/test_pycurves.py` & `openpile-0.3.1/test/test_pycurves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.3.0/test/test_utils_misc.py` & `openpile-0.3.1/test/test_utils_misc.py`

 * *Files identical despite different names*

