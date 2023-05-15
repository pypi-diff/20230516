# Comparing `tmp/astro-elk-0.3.tar.gz` & `tmp/astro-elk-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-elk-0.3.tar", last modified: Mon May 15 22:19:58 2023, max compression
+gzip compressed data, was "astro-elk-0.4.tar", last modified: Mon May 15 22:48:03 2023, max compression
```

## Comparing `astro-elk-0.3.tar` & `astro-elk-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:19:58.315995 astro-elk-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 22:19:58.315995 astro-elk-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-15 22:19:47.000000 astro-elk-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:19:58.315995 astro-elk-0.3/astro_elk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 22:19:58.000000 astro-elk-0.3/astro_elk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 22:19:58.000000 astro-elk-0.3/astro_elk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:19:58.000000 astro-elk-0.3/astro_elk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 22:19:58.000000 astro-elk-0.3/astro_elk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 22:19:58.000000 astro-elk-0.3/astro_elk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:19:58.315995 astro-elk-0.3/elk/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 22:19:47.000000 astro-elk-0.3/elk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 22:19:47.000000 astro-elk-0.3/elk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-05-15 22:19:47.000000 astro-elk-0.3/elk/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-15 22:19:47.000000 astro-elk-0.3/elk/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-15 22:19:47.000000 astro-elk-0.3/elk/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-15 22:19:47.000000 astro-elk-0.3/elk/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-15 22:19:47.000000 astro-elk-0.3/elk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 22:19:58.315995 astro-elk-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 22:19:47.000000 astro-elk-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:48:03.419259 astro-elk-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 22:48:03.419259 astro-elk-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-15 22:47:53.000000 astro-elk-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:48:03.419259 astro-elk-0.4/astro_elk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 22:48:03.000000 astro-elk-0.4/astro_elk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 22:48:03.000000 astro-elk-0.4/astro_elk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:48:03.000000 astro-elk-0.4/astro_elk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 22:48:03.000000 astro-elk-0.4/astro_elk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 22:48:03.000000 astro-elk-0.4/astro_elk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:48:03.419259 astro-elk-0.4/elk/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 22:47:53.000000 astro-elk-0.4/elk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 22:47:53.000000 astro-elk-0.4/elk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22521 2023-05-15 22:47:53.000000 astro-elk-0.4/elk/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-15 22:47:53.000000 astro-elk-0.4/elk/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-15 22:47:53.000000 astro-elk-0.4/elk/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-15 22:47:53.000000 astro-elk-0.4/elk/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-15 22:47:53.000000 astro-elk-0.4/elk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 22:48:03.419259 astro-elk-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 22:47:53.000000 astro-elk-0.4/setup.py
```

### Comparing `astro-elk-0.3/PKG-INFO` & `astro-elk-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-elk
-Version: 0.3
+Version: 0.4
 Summary: This python package computes, and corrects ensemble light curves for TESS pixels within a specified aperature, from TESS FFI data.
 Home-page: https://github.com/tobin-wainer/TESS_Cluster_Project/
 Author: Tobin Wainer, Tom Wagg
 Author-email: tobinw@uw.edu
 License: MIT
 Platform: UNKNOWN
 Provides: elk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astro-elk Version: 0.3 Summary: This python package
+Metadata-Version: 2.1 Name: astro-elk Version: 0.4 Summary: This python package
 computes, and corrects ensemble light curves for TESS pixels within a specified
 aperature, from TESS FFI data. Home-page: https://github.com/tobin-wainer/
 TESS_Cluster_Project/ Author: Tobin Wainer, Tom Wagg Author-email:
 tobinw@uw.edu License: MIT Platform: UNKNOWN Provides: elk Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Provides-Extra: test Provides-
 Extra: docs
    src="https://raw.githubusercontent.com/tobin-wainer/elk/main/docs/_static/
```

### Comparing `astro-elk-0.3/README.md` & `astro-elk-0.4/README.md`

 * *Files identical despite different names*

### Comparing `astro-elk-0.3/astro_elk.egg-info/PKG-INFO` & `astro-elk-0.4/astro_elk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-elk
-Version: 0.3
+Version: 0.4
 Summary: This python package computes, and corrects ensemble light curves for TESS pixels within a specified aperature, from TESS FFI data.
 Home-page: https://github.com/tobin-wainer/TESS_Cluster_Project/
 Author: Tobin Wainer, Tom Wagg
 Author-email: tobinw@uw.edu
 License: MIT
 Platform: UNKNOWN
 Provides: elk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astro-elk Version: 0.3 Summary: This python package
+Metadata-Version: 2.1 Name: astro-elk Version: 0.4 Summary: This python package
 computes, and corrects ensemble light curves for TESS pixels within a specified
 aperature, from TESS FFI data. Home-page: https://github.com/tobin-wainer/
 TESS_Cluster_Project/ Author: Tobin Wainer, Tom Wagg Author-email:
 tobinw@uw.edu License: MIT Platform: UNKNOWN Provides: elk Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Provides-Extra: test Provides-
 Extra: docs
    src="https://raw.githubusercontent.com/tobin-wainer/elk/main/docs/_static/
```

### Comparing `astro-elk-0.3/elk/ensemble.py` & `astro-elk-0.4/elk/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,17 @@
                       'scattered_light_sectors': [self.scattered_light_sectors if len(self.scattered_light_sectors) > 0 else 0],
                       'lc_lens': [[len(lc.corrected_lc) for lc in self.lcs if lc is not None]]})
 
 
 def from_fits(filepath, existing_class=None, **kwargs):
     # if an existing class is not provided then create a new blank one
     if existing_class is None:
-        new_ecl = EnsembleLC(identifier="", radius=None, cluster_age=None, output_path=None, **kwargs)
+        # work out what the output path is based on the filepath input
+        output_path = os.path.join(*filepath.split("/")[:-2])
+        new_ecl = EnsembleLC(identifier="", radius=None, cluster_age=None, output_path=output_path, **kwargs)
     else:
         new_ecl = existing_class
 
     # open up the fits file and load in the information
     with fits.open(filepath) as hdul:
         details = hdul[0]
         new_ecl.identifier = details.header["name"]
```

### Comparing `astro-elk-0.3/elk/lightcurve.py` & `astro-elk-0.4/elk/lightcurve.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.3/elk/plot.py` & `astro-elk-0.4/elk/plot.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.3/elk/stats.py` & `astro-elk-0.4/elk/stats.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.3/elk/utils.py` & `astro-elk-0.4/elk/utils.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.3/setup.cfg` & `astro-elk-0.4/setup.cfg`

 * *Files identical despite different names*

