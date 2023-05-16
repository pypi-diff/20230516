# Comparing `tmp/lisflood-lisvap-1.2.6.tar.gz` & `tmp/lisflood-lisvap-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lisflood-lisvap-1.2.6.tar", last modified: Thu Mar 16 16:32:51 2023, max compression
+gzip compressed data, was "dist/lisflood-lisvap-1.2.7.tar", last modified: Tue May 16 15:03:01 2023, max compression
```

## Comparing `lisflood-lisvap-1.2.6.tar` & `lisflood-lisvap-1.2.7.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)       14 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/MANIFEST.in
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3724 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/PKG-INFO
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     2041 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/README.md
-drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/bin/
--rwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)      281 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/bin/lisvap
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    16495 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/settings_tpl.xml
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)       38 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/setup.cfg
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     4652 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/setup.py
-drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/
-drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisflood_lisvap.egg-info/
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3724 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisflood_lisvap.egg-info/PKG-INFO
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)      752 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisflood_lisvap.egg-info/SOURCES.txt
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)        1 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisflood_lisvap.egg-info/dependency_links.txt
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)       57 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisflood_lisvap.egg-info/requires.txt
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)       15 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisflood_lisvap.egg-info/top_level.txt
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)        1 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisflood_lisvap.egg-info/zip-safe
-drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisvap/
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)      345 2023-03-16 16:32:17.000000 lisflood-lisvap-1.2.6/src/lisvap/__init__.py
-drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisvap/hydrological/
--rwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/hydrological/__init__.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3609 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/hydrological/miscinitial.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     7493 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/hydrological/readmeteo.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    10922 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/lisvapdynamic.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3498 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/lisvapinitial.py
-drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.6/src/lisvap/utils/
--rwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)    27404 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/utils/__init__.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     1129 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/utils/decorators.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     2232 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/utils/defaults_options.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)      620 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/utils/operators.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    12653 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/utils/output.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    18007 2023-03-16 16:32:17.000000 lisflood-lisvap-1.2.6/src/lisvap/utils/readers.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    10476 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/utils/tools.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    12117 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap/utils/writers.py
--rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3467 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.6/src/lisvap1.py
+drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    13760 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/LICENSE
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)       14 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/MANIFEST.in
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3459 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/PKG-INFO
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     2041 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/README.md
+drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/bin/
+-rwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)      281 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/bin/lisvap
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    16495 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/settings_tpl.xml
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)       38 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/setup.cfg
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     4652 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/setup.py
+drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/
+drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/lisflood_lisvap.egg-info/
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3459 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/lisflood_lisvap.egg-info/PKG-INFO
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)      760 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/lisflood_lisvap.egg-info/SOURCES.txt
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)        1 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/lisflood_lisvap.egg-info/dependency_links.txt
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)       57 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/lisflood_lisvap.egg-info/requires.txt
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)       15 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/lisflood_lisvap.egg-info/top_level.txt
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)        1 2023-03-16 16:32:51.000000 lisflood-lisvap-1.2.7/src/lisflood_lisvap.egg-info/zip-safe
+drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/lisvap/
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)      345 2023-05-16 14:59:26.000000 lisflood-lisvap-1.2.7/src/lisvap/__init__.py
+drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/lisvap/hydrological/
+-rwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/hydrological/__init__.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3609 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/hydrological/miscinitial.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     7493 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/hydrological/readmeteo.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    10922 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/lisvapdynamic.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3498 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/lisvapinitial.py
+drwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)        0 2023-05-16 15:03:01.000000 lisflood-lisvap-1.2.7/src/lisvap/utils/
+-rwxrwxr-x   0 gomesgl   (1002) gomesgl   (1003)    27404 2023-05-16 14:17:06.000000 lisflood-lisvap-1.2.7/src/lisvap/utils/__init__.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     1129 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/utils/decorators.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     2232 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/utils/defaults_options.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)      620 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/utils/operators.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    12653 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/utils/output.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    18248 2023-05-16 14:59:26.000000 lisflood-lisvap-1.2.7/src/lisvap/utils/readers.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    10476 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/utils/tools.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)    12117 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap/utils/writers.py
+-rw-rw-r--   0 gomesgl   (1002) gomesgl   (1003)     3467 2023-03-16 14:53:29.000000 lisflood-lisvap-1.2.7/src/lisvap1.py
```

### Comparing `lisflood-lisvap-1.2.6/PKG-INFO` & `lisflood-lisvap-1.2.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,16 @@
 Metadata-Version: 2.1
 Name: lisflood-lisvap
-Version: 1.2.6
+Version: 1.2.7
 Summary: LISVAP model python module
 Home-page: https://github.com/ec-jrc/lisflood-lisvap
 Author: Ad de Roo, Peter Burek, Johan van der Knijff, Domenico Nappo
 Author-email: domenico.nappo@ext.ec.europa.eu
 License: EUPL 1.2
-Description: # Lisflood OS
-        
-        This repository hosts source code of LISVAP model.
-        Go to [Lisflood OS page](https://ec-jrc.github.io/lisflood/) for more information.
-        
-        Other useful resources
-        
-        | **Project**         | **Documentation**                                         | **Source code**                                              |
-        | ------------------- | --------------------------------------------------------- | ------------------------------------------------------------ |
-        | Lisflood            | [Model docs](https://ec-jrc.github.io/lisflood-model/)    | https://github.com/ec-jrc/lisflood-code                      |
-        |                     | [User guide](https://ec-jrc.github.io/lisflood-code/)     |                                                              |
-        | Lisvap              | [Docs](https://ec-jrc.github.io/lisflood-lisvap/)         | https://github.com/ec-jrc/lisflood-lisvap (this repository)  |
-        | Calibration tool    | [Docs](https://ec-jrc.github.io/lisflood-calibration/)    | https://github.com/ec-jrc/lisflood-calibration               |
-        | Lisflood Utilities  |                                                           | https://github.com/ec-jrc/lisflood-utilities                 |
-        | Lisflood Usecases   |                                                           | https://github.com/ec-jrc/lisflood-usecases                  |
-        
-        
-        
-        ## LISVAP
-        
-        LISVAP is a model that produce Evaporation timeseries maps that can be used as input to Water Balance/Flood simulation models.
-        
-        Reference values for potential evapotranspiration and evaporation are estimated using the Penman-Monteith equation (Supit et al., 1994, Supit & Van Der Goot, 2003)
-        
-        
-        For full documentation, please visit the [official documentation](https://ec-jrc.github.io/lisflood-lisvap/) website.
-        
-        This software is part of Lisflood Open source/Nexus Initiative and it's released under the EUPL 1.2 license.
-        Source code and test cases are available in the [LISVAP GitHub repository](https://github.com/ec-jrc/lisflood-lisvap/)
-        JRC - European Commission
-        
-        (C) 2019
-        
 Keywords: lisflood lisvap efas evapotranspiration evaporation
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -58,7 +24,41 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=2.7,!=3.0.*,!=3.1.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Lisflood OS
+
+This repository hosts source code of LISVAP model.
+Go to [Lisflood OS page](https://ec-jrc.github.io/lisflood/) for more information.
+
+Other useful resources
+
+| **Project**         | **Documentation**                                         | **Source code**                                              |
+| ------------------- | --------------------------------------------------------- | ------------------------------------------------------------ |
+| Lisflood            | [Model docs](https://ec-jrc.github.io/lisflood-model/)    | https://github.com/ec-jrc/lisflood-code                      |
+|                     | [User guide](https://ec-jrc.github.io/lisflood-code/)     |                                                              |
+| Lisvap              | [Docs](https://ec-jrc.github.io/lisflood-lisvap/)         | https://github.com/ec-jrc/lisflood-lisvap (this repository)  |
+| Calibration tool    | [Docs](https://ec-jrc.github.io/lisflood-calibration/)    | https://github.com/ec-jrc/lisflood-calibration               |
+| Lisflood Utilities  |                                                           | https://github.com/ec-jrc/lisflood-utilities                 |
+| Lisflood Usecases   |                                                           | https://github.com/ec-jrc/lisflood-usecases                  |
+
+
+
+## LISVAP
+
+LISVAP is a model that produce Evaporation timeseries maps that can be used as input to Water Balance/Flood simulation models.
+
+Reference values for potential evapotranspiration and evaporation are estimated using the Penman-Monteith equation (Supit et al., 1994, Supit & Van Der Goot, 2003)
+
+
+For full documentation, please visit the [official documentation](https://ec-jrc.github.io/lisflood-lisvap/) website.
+
+This software is part of Lisflood Open source/Nexus Initiative and it's released under the EUPL 1.2 license.
+Source code and test cases are available in the [LISVAP GitHub repository](https://github.com/ec-jrc/lisflood-lisvap/)
+JRC - European Commission
+
+(C) 2019
```

### Comparing `lisflood-lisvap-1.2.6/README.md` & `lisflood-lisvap-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/settings_tpl.xml` & `lisflood-lisvap-1.2.7/settings_tpl.xml`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/setup.py` & `lisflood-lisvap-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisflood_lisvap.egg-info/PKG-INFO` & `lisflood-lisvap-1.2.7/src/lisflood_lisvap.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,16 @@
 Metadata-Version: 2.1
 Name: lisflood-lisvap
-Version: 1.2.6
+Version: 1.2.7
 Summary: LISVAP model python module
 Home-page: https://github.com/ec-jrc/lisflood-lisvap
 Author: Ad de Roo, Peter Burek, Johan van der Knijff, Domenico Nappo
 Author-email: domenico.nappo@ext.ec.europa.eu
 License: EUPL 1.2
-Description: # Lisflood OS
-        
-        This repository hosts source code of LISVAP model.
-        Go to [Lisflood OS page](https://ec-jrc.github.io/lisflood/) for more information.
-        
-        Other useful resources
-        
-        | **Project**         | **Documentation**                                         | **Source code**                                              |
-        | ------------------- | --------------------------------------------------------- | ------------------------------------------------------------ |
-        | Lisflood            | [Model docs](https://ec-jrc.github.io/lisflood-model/)    | https://github.com/ec-jrc/lisflood-code                      |
-        |                     | [User guide](https://ec-jrc.github.io/lisflood-code/)     |                                                              |
-        | Lisvap              | [Docs](https://ec-jrc.github.io/lisflood-lisvap/)         | https://github.com/ec-jrc/lisflood-lisvap (this repository)  |
-        | Calibration tool    | [Docs](https://ec-jrc.github.io/lisflood-calibration/)    | https://github.com/ec-jrc/lisflood-calibration               |
-        | Lisflood Utilities  |                                                           | https://github.com/ec-jrc/lisflood-utilities                 |
-        | Lisflood Usecases   |                                                           | https://github.com/ec-jrc/lisflood-usecases                  |
-        
-        
-        
-        ## LISVAP
-        
-        LISVAP is a model that produce Evaporation timeseries maps that can be used as input to Water Balance/Flood simulation models.
-        
-        Reference values for potential evapotranspiration and evaporation are estimated using the Penman-Monteith equation (Supit et al., 1994, Supit & Van Der Goot, 2003)
-        
-        
-        For full documentation, please visit the [official documentation](https://ec-jrc.github.io/lisflood-lisvap/) website.
-        
-        This software is part of Lisflood Open source/Nexus Initiative and it's released under the EUPL 1.2 license.
-        Source code and test cases are available in the [LISVAP GitHub repository](https://github.com/ec-jrc/lisflood-lisvap/)
-        JRC - European Commission
-        
-        (C) 2019
-        
 Keywords: lisflood lisvap efas evapotranspiration evaporation
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -58,7 +24,41 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=2.7,!=3.0.*,!=3.1.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Lisflood OS
+
+This repository hosts source code of LISVAP model.
+Go to [Lisflood OS page](https://ec-jrc.github.io/lisflood/) for more information.
+
+Other useful resources
+
+| **Project**         | **Documentation**                                         | **Source code**                                              |
+| ------------------- | --------------------------------------------------------- | ------------------------------------------------------------ |
+| Lisflood            | [Model docs](https://ec-jrc.github.io/lisflood-model/)    | https://github.com/ec-jrc/lisflood-code                      |
+|                     | [User guide](https://ec-jrc.github.io/lisflood-code/)     |                                                              |
+| Lisvap              | [Docs](https://ec-jrc.github.io/lisflood-lisvap/)         | https://github.com/ec-jrc/lisflood-lisvap (this repository)  |
+| Calibration tool    | [Docs](https://ec-jrc.github.io/lisflood-calibration/)    | https://github.com/ec-jrc/lisflood-calibration               |
+| Lisflood Utilities  |                                                           | https://github.com/ec-jrc/lisflood-utilities                 |
+| Lisflood Usecases   |                                                           | https://github.com/ec-jrc/lisflood-usecases                  |
+
+
+
+## LISVAP
+
+LISVAP is a model that produce Evaporation timeseries maps that can be used as input to Water Balance/Flood simulation models.
+
+Reference values for potential evapotranspiration and evaporation are estimated using the Penman-Monteith equation (Supit et al., 1994, Supit & Van Der Goot, 2003)
+
+
+For full documentation, please visit the [official documentation](https://ec-jrc.github.io/lisflood-lisvap/) website.
+
+This software is part of Lisflood Open source/Nexus Initiative and it's released under the EUPL 1.2 license.
+Source code and test cases are available in the [LISVAP GitHub repository](https://github.com/ec-jrc/lisflood-lisvap/)
+JRC - European Commission
+
+(C) 2019
```

### Comparing `lisflood-lisvap-1.2.6/src/lisflood_lisvap.egg-info/SOURCES.txt` & `lisflood-lisvap-1.2.7/src/lisflood_lisvap.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 settings_tpl.xml
 setup.py
 bin/lisvap
 src/lisvap1.py
 src/lisflood_lisvap.egg-info/PKG-INFO
```

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/hydrological/miscinitial.py` & `lisflood-lisvap-1.2.7/src/lisvap/hydrological/miscinitial.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/hydrological/readmeteo.py` & `lisflood-lisvap-1.2.7/src/lisvap/hydrological/readmeteo.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/lisvapdynamic.py` & `lisflood-lisvap-1.2.7/src/lisvap/lisvapdynamic.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/lisvapinitial.py` & `lisflood-lisvap-1.2.7/src/lisvap/lisvapinitial.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/utils/__init__.py` & `lisflood-lisvap-1.2.7/src/lisvap/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/utils/decorators.py` & `lisflood-lisvap-1.2.7/src/lisvap/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/utils/defaults_options.py` & `lisflood-lisvap-1.2.7/src/lisvap/utils/defaults_options.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/utils/operators.py` & `lisflood-lisvap-1.2.7/src/lisvap/utils/operators.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/utils/output.py` & `lisflood-lisvap-1.2.7/src/lisvap/utils/output.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/utils/readers.py` & `lisflood-lisvap-1.2.7/src/lisvap/utils/readers.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             iter_setclone_pcraster(filename)
             res = operations.boolean(iter_read_pcraster(filename))
             flagmap = True
         except:
             # try to read a netcdf file
             filename = '{}.{}'.format(os.path.splitext(settings.binding[name])[0], 'nc')
             nf1 = iter_open_netcdf(filename, 'r')
-            value = listitems(nf1.variables)[-1][0]  # get the last variable name
+            value = get_netcdf_meteo_variable_name(nf1)
 
             x_var = 'x'
             y_var = 'y'
             if 'lon' in nf1.variables.keys():
                 x_var = 'lon'
                 y_var = 'lat'
             x1 = Decimal(__DECIMAL_FORMAT.format(nf1.variables[x_var][0]))
@@ -141,15 +141,15 @@
 
         # get mapextend of netcdf map
         # and calculate the cutting
         cut0, cut1, cut2, cut3 = CutMap.get_cuts(filename)
 
         # load netcdf map but only the rectangle needed
         nf1 = Dataset(filename, 'r')
-        value = listitems(nf1.variables)[-1][0]  # get the last variable name
+        value = get_netcdf_meteo_variable_name(nf1)
         mapnp = nf1.variables[value][cut2:cut3, cut0:cut1]
         nf1.close()
 
         # check if integer map (like outlets, lakes etc)
         checkint = str(mapnp.dtype)
         if checkint == "int16" or checkint == "int32":
             mapnp[mapnp.mask] = -9999
@@ -356,14 +356,21 @@
         simulation last date: {}
         """.format(filename, date_last_step_in_ncdf.strftime('%d/%m/%Y %H:%M'), date_last_sim_step.strftime('%d/%m/%Y %H:%M'))
         raise LisfloodError(msg)
 
     return
 
 
+def get_netcdf_meteo_variable_name(nc_file_obj):
+    # Only one variable must be present in netcdf files
+    num_dims = 3 if 'time' in nc_file_obj.variables else 2
+    varname = [v for v in nc_file_obj.variables if len(nc_file_obj.variables[v].dimensions) == num_dims][0]
+    return varname
+
+
 def iter_open_netcdf(file_path, mode, **kwargs):
     """Wrapper around netCDF4.Dataset function exploiting the iterAccess class to access file_path according to the specified mode"""
     def access_function(path):
         return Dataset(path, mode, **kwargs)
     return remote_input_access(access_function, file_path)
```

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/utils/tools.py` & `lisflood-lisvap-1.2.7/src/lisvap/utils/tools.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap/utils/writers.py` & `lisflood-lisvap-1.2.7/src/lisvap/utils/writers.py`

 * *Files identical despite different names*

### Comparing `lisflood-lisvap-1.2.6/src/lisvap1.py` & `lisflood-lisvap-1.2.7/src/lisvap1.py`

 * *Files identical despite different names*

