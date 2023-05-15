# Comparing `tmp/astro-elk-0.5.tar.gz` & `tmp/astro-elk-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-elk-0.5.tar", last modified: Mon May 15 22:57:25 2023, max compression
+gzip compressed data, was "astro-elk-0.6.tar", last modified: Mon May 15 23:23:09 2023, max compression
```

## Comparing `astro-elk-0.5.tar` & `astro-elk-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:57:25.572787 astro-elk-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 22:57:25.572787 astro-elk-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-15 22:57:09.000000 astro-elk-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:57:25.568787 astro-elk-0.5/astro_elk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 22:57:25.000000 astro-elk-0.5/astro_elk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 22:57:25.000000 astro-elk-0.5/astro_elk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:57:25.000000 astro-elk-0.5/astro_elk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 22:57:25.000000 astro-elk-0.5/astro_elk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 22:57:25.000000 astro-elk-0.5/astro_elk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:57:25.572787 astro-elk-0.5/elk/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 22:57:09.000000 astro-elk-0.5/elk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 22:57:09.000000 astro-elk-0.5/elk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22596 2023-05-15 22:57:09.000000 astro-elk-0.5/elk/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-15 22:57:09.000000 astro-elk-0.5/elk/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-15 22:57:09.000000 astro-elk-0.5/elk/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-15 22:57:09.000000 astro-elk-0.5/elk/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-15 22:57:09.000000 astro-elk-0.5/elk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 22:57:25.572787 astro-elk-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 22:57:09.000000 astro-elk-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:23:09.097237 astro-elk-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 23:23:09.097237 astro-elk-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-15 23:22:58.000000 astro-elk-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:23:09.097237 astro-elk-0.6/astro_elk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-15 23:23:09.000000 astro-elk-0.6/astro_elk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 23:23:09.000000 astro-elk-0.6/astro_elk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:23:09.000000 astro-elk-0.6/astro_elk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 23:23:09.000000 astro-elk-0.6/astro_elk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 23:23:09.000000 astro-elk-0.6/astro_elk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:23:09.097237 astro-elk-0.6/elk/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 23:22:58.000000 astro-elk-0.6/elk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 23:22:58.000000 astro-elk-0.6/elk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22607 2023-05-15 23:22:58.000000 astro-elk-0.6/elk/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-15 23:22:58.000000 astro-elk-0.6/elk/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-15 23:22:58.000000 astro-elk-0.6/elk/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-15 23:22:58.000000 astro-elk-0.6/elk/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-15 23:22:58.000000 astro-elk-0.6/elk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 23:23:09.097237 astro-elk-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 23:22:58.000000 astro-elk-0.6/setup.py
```

### Comparing `astro-elk-0.5/PKG-INFO` & `astro-elk-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-elk
-Version: 0.5
+Version: 0.6
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
-Metadata-Version: 2.1 Name: astro-elk Version: 0.5 Summary: This python package
+Metadata-Version: 2.1 Name: astro-elk Version: 0.6 Summary: This python package
 computes, and corrects ensemble light curves for TESS pixels within a specified
 aperature, from TESS FFI data. Home-page: https://github.com/tobin-wainer/
 TESS_Cluster_Project/ Author: Tobin Wainer, Tom Wagg Author-email:
 tobinw@uw.edu License: MIT Platform: UNKNOWN Provides: elk Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Provides-Extra: test Provides-
 Extra: docs
    src="https://raw.githubusercontent.com/tobin-wainer/elk/main/docs/_static/
```

### Comparing `astro-elk-0.5/README.md` & `astro-elk-0.6/README.md`

 * *Files identical despite different names*

### Comparing `astro-elk-0.5/astro_elk.egg-info/PKG-INFO` & `astro-elk-0.6/astro_elk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-elk
-Version: 0.5
+Version: 0.6
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
-Metadata-Version: 2.1 Name: astro-elk Version: 0.5 Summary: This python package
+Metadata-Version: 2.1 Name: astro-elk Version: 0.6 Summary: This python package
 computes, and corrects ensemble light curves for TESS pixels within a specified
 aperature, from TESS FFI data. Home-page: https://github.com/tobin-wainer/
 TESS_Cluster_Project/ Author: Tobin Wainer, Tom Wagg Author-email:
 tobinw@uw.edu License: MIT Platform: UNKNOWN Provides: elk Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Provides-Extra: test Provides-
 Extra: docs
    src="https://raw.githubusercontent.com/tobin-wainer/elk/main/docs/_static/
```

### Comparing `astro-elk-0.5/elk/ensemble.py` & `astro-elk-0.6/elk/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,16 +425,16 @@
         # return a simple summary table that can be conveniently stacked with other clusters
         return Table({'name': [self.identifier], 'location': [self.location], 'radius': [self.radius],
                       'log_age': [self.cluster_age], 'has_data': [self.sectors_available > 0],
                       'n_obs': [self.sectors_available], 'n_good_obs': [self.n_good_obs],
                       'which_sectors_good': [[lc.sector for lc in self.lcs if lc is not None]],
                       'n_failed_download': [self.n_failed_download], 'n_bad_quality': [self.n_bad_quality],
                       'n_scatter_light': [len(self.scattered_light_sectors)],
-                      'scattered_light_sectors': [self.scattered_light_sectors if len(self.scattered_light_sectors) > 0 else 0],
-                      'lc_lens': [[len(lc.corrected_lc) for lc in self.lcs if lc is not None]]})
+                      'scattered_light_sectors': [self.scattered_light_sectors if len(self.scattered_light_sectors) > 0 else -99],
+                      'lc_lens': [[len(lc.corrected_lc) for lc in self.lcs if lc is not None else -99]]})
 
 
 def from_fits(filepath, existing_class=None, **kwargs):
     # if an existing class is not provided then create a new blank one
     if existing_class is None:
         # work out what the output path is based on the filepath input
         output_path = os.path.join(*filepath.split("/")[:-2])
```

### Comparing `astro-elk-0.5/elk/lightcurve.py` & `astro-elk-0.6/elk/lightcurve.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.5/elk/plot.py` & `astro-elk-0.6/elk/plot.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.5/elk/stats.py` & `astro-elk-0.6/elk/stats.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.5/elk/utils.py` & `astro-elk-0.6/elk/utils.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.5/setup.cfg` & `astro-elk-0.6/setup.cfg`

 * *Files identical despite different names*

