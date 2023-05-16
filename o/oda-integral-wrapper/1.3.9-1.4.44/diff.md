# Comparing `tmp/oda_integral_wrapper-1.3.9.tar.gz` & `tmp/oda_integral_wrapper-1.4.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oda_integral_wrapper-1.3.9.tar", last modified: Tue Apr 27 19:58:22 2021, max compression
+gzip compressed data, was "oda_integral_wrapper-1.4.44.tar", last modified: Tue May 16 20:55:57 2023, max compression
```

## Comparing `oda_integral_wrapper-1.3.9.tar` & `oda_integral_wrapper-1.4.44.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 ferrigno  (1001) ferrigno  (1001)        0 2021-04-27 19:58:22.312028 oda_integral_wrapper-1.3.9/
--rw-rw-r--   0 ferrigno  (1001) ferrigno  (1001)      367 2021-04-27 19:58:22.312028 oda_integral_wrapper-1.3.9/PKG-INFO
--rw-r--r--   0 ferrigno  (1001) ferrigno  (1001)     1890 2021-03-04 23:47:29.000000 oda_integral_wrapper-1.3.9/README.md
-drwxrwxr-x   0 ferrigno  (1001) ferrigno  (1001)        0 2021-04-27 19:58:22.312028 oda_integral_wrapper-1.3.9/oda_integral_wrapper/
--rw-r--r--   0 ferrigno  (1001) ferrigno  (1001)      751 2020-06-11 08:22:33.000000 oda_integral_wrapper-1.3.9/oda_integral_wrapper/__init__.py
--rw-rw-r--   0 ferrigno  (1001) ferrigno  (1001)     5988 2020-06-11 14:53:53.000000 oda_integral_wrapper-1.3.9/oda_integral_wrapper/fitimage.py
--rw-rw-r--   0 ferrigno  (1001) ferrigno  (1001)    49501 2021-04-27 19:56:18.000000 oda_integral_wrapper-1.3.9/oda_integral_wrapper/wrapper.py
-drwxrwxr-x   0 ferrigno  (1001) ferrigno  (1001)        0 2021-04-27 19:58:22.312028 oda_integral_wrapper-1.3.9/oda_integral_wrapper.egg-info/
--rw-r--r--   0 ferrigno  (1001) ferrigno  (1001)      367 2021-04-27 19:58:22.000000 oda_integral_wrapper-1.3.9/oda_integral_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 ferrigno  (1001) ferrigno  (1001)      345 2021-04-27 19:58:22.000000 oda_integral_wrapper-1.3.9/oda_integral_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 ferrigno  (1001) ferrigno  (1001)        1 2021-04-27 19:58:22.000000 oda_integral_wrapper-1.3.9/oda_integral_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 ferrigno  (1001) ferrigno  (1001)       85 2021-04-27 19:58:22.000000 oda_integral_wrapper-1.3.9/oda_integral_wrapper.egg-info/requires.txt
--rw-r--r--   0 ferrigno  (1001) ferrigno  (1001)       21 2021-04-27 19:58:22.000000 oda_integral_wrapper-1.3.9/oda_integral_wrapper.egg-info/top_level.txt
--rw-r--r--   0 ferrigno  (1001) ferrigno  (1001)       79 2021-04-27 19:58:22.312028 oda_integral_wrapper-1.3.9/setup.cfg
--rw-rw-r--   0 ferrigno  (1001) ferrigno  (1001)     1288 2021-04-27 19:56:18.000000 oda_integral_wrapper-1.3.9/setup.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-16 20:55:57.163560 oda_integral_wrapper-1.4.44/
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)     1175 2021-02-19 13:03:51.000000 oda_integral_wrapper-1.4.44/LICENSE.rst
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      338 2023-05-16 20:55:57.163560 oda_integral_wrapper-1.4.44/PKG-INFO
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)     1890 2021-03-04 23:47:29.000000 oda_integral_wrapper-1.4.44/README.md
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-16 20:55:57.163560 oda_integral_wrapper-1.4.44/oda_integral_wrapper/
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)      794 2021-04-28 13:12:46.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper/__init__.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    15570 2021-10-08 11:47:27.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper/fit_cyclotron.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     6114 2022-06-17 12:23:32.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper/fitimage.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     8623 2021-04-30 07:41:48.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper/get_osa10_11_factor.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     3238 2022-08-05 07:47:15.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper/itime.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    18177 2023-05-16 20:54:17.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper/planning.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    79198 2023-04-06 16:39:21.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper/wrapper.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-16 20:55:57.163560 oda_integral_wrapper-1.4.44/oda_integral_wrapper.egg-info/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      338 2023-05-16 20:55:57.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      502 2023-05-16 20:55:57.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2023-05-16 20:55:57.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       92 2023-05-16 20:55:57.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       21 2023-05-16 20:55:57.000000 oda_integral_wrapper-1.4.44/oda_integral_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)       79 2023-05-16 20:55:57.167559 oda_integral_wrapper-1.4.44/setup.cfg
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1197 2023-05-16 20:55:39.000000 oda_integral_wrapper-1.4.44/setup.py
```

### Comparing `oda_integral_wrapper-1.3.9/README.md` & `oda_integral_wrapper-1.4.44/README.md`

 * *Files identical despite different names*

### Comparing `oda_integral_wrapper-1.3.9/oda_integral_wrapper/fitimage.py` & `oda_integral_wrapper-1.4.44/oda_integral_wrapper/fitimage.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 __author__ = "Volodymyr Savchenko"
 
 __all__ = ['FitMosaicSources']
 
 class FitMosaicSources(object):
 
-    def __init__(self, mosaic_hdulist, cat):
+    def __init__(self, mosaic_hdulist, cat, free_sigma=False, free_constant=False):
 
     #cat=[('Tycho SNR',(6.3583,64.1528))]
     #cat=[('Cas A',(350.85,58.810))]
 
         self.cat = cat
         self.mosaic_hdu_list = mosaic_hdulist
         self.fluxes = ones(len(cat))
         self.radius = 5
-        self.free_constant = False
+        self.free_constant = free_constant
         self.usexy = False
         self.sigma = 1.1578793
-        self.free_sigma = False
+        self.free_sigma = free_sigma
 
     def model(self):
         if not hasattr(self, 'wcs'):
             raise RuntimeError('No WCS attribute')
 
        # print("data shape",self.data_shape)
 
@@ -84,22 +84,22 @@
         return model, mask
 
     def fit_image(self,rate,variance):
 
         import nlopt
 
         def myfunc(x, grad):
-            #print(":::::::", x)
+            # print(":::::::", x)
 
             if self.free_sigma:
                 self.sigma = x[0]
                 x = x[1:]
 
             if self.free_constant:
-                self.constant=x[0]
+                self.constant = x[0]
                 x = x[1:]
 
             #
             # The fitting variable, passed to model implicitly !
             #
             self.fluxes = x[:]
 
@@ -108,36 +108,34 @@
             self.residuals = r
             self.residuals[~mask] = 0
             ndof = r[mask].flatten().shape[0]
             residual = (r[mask]**2).sum()/ndof
             #print("------------->", x, local_model.sum(), residual, ndof, residual/ndof)
             return residual
 
-
-
-        #self.free_constant=True
-
         x0 = []
         xmin = []
         xmax = []
 
         if self.free_sigma:
             x0.append(1)
             xmin.append(0.1)
             xmax.append(2)
         
         if self.free_constant:
             x0.append(0)
             xmin.append(-10)
             xmax.append(10)
+            self.constant = 0.
+            #print('SETTING')
 
         x0 += [0]*len(self.fluxes)
 
         loc_mod, loc_mask = self.model()
-        #print(3 * (array(rate[loc_mask]).max()))
+        # print(3 * (array(rate[loc_mask]).max()))
 
         xmin += [-5*array(rate[loc_mask]).max()]*len(self.fluxes)
         xmax += [10*array(rate[loc_mask]).max()]*len(self.fluxes)
 
         opt = nlopt.opt(nlopt.LN_BOBYQA, len(x0))
         #opt = nlopt.opt(nlopt.LN_COBYLA, len(x0))
         opt.set_lower_bounds(xmin)
@@ -182,15 +180,15 @@
         #
         f = self.mosaic_hdu_list
 
         intensity_i = []
         variance_i = []
 
         for ie, e in enumerate(f):
-            if 'IMATYPE' in e.header and e.header['IMATYPE'] == "INTENSITY":
+            if 'IMATYPE' in e.header and ( e.header['IMATYPE'] == "INTENSITY" or e.header['IMATYPE'] == "RECONSTRUCTED"):
                     intensity_i.append(ie)
 
             if 'IMATYPE' in e.header and e.header['IMATYPE'] == "VARIANCE":
                     variance_i.append(ie)
 
         spectra = []
         src_names = [cc[0] for cc in self.cat]
```

### Comparing `oda_integral_wrapper-1.3.9/setup.py` & `oda_integral_wrapper-1.4.44/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-
 from __future__ import absolute_import, division, print_function
 
-from builtins import (bytes, str, open, super, range,
-                      zip, round, input, int, pow, object, map, zip)
-
 __author__ = 'Carlo Ferrigno'
 
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
-import  glob
+import glob
 
-packs=find_packages()
+packs = find_packages()
 
-print ('packs',packs)
+print('packs', packs)
 
-include_package_data=True
+include_package_data = True
 
 scripts_list = glob.glob('./bin/*')
 setup(name='oda_integral_wrapper',
-      version="1.3.9",
+      version="1.4.44",
       description='wrapper for INTEGRAL analysis using the API plugin for CDCI online data analysis',
       author='Carlo Ferrigno',
       author_email='carlo.ferrigno@unige.ch',
       url="https://gitlab.astro.unige.ch/oda/api-clients/oda_api_wrapper",
       scripts=scripts_list,
       packages=packs,
-      package_data={'oda_integral_wrapper' : ['config_dir/*']},
+      package_data={'oda_integral_wrapper': ['config_dir/*']},
       include_package_data=True,
       install_requires=[
                         "astropy",
                         "matplotlib",
                         "numpy",
                         "oda_api",
                         "requests",
                         "astroquery",
                         "pymosaic-fits",
                         "nlopt",
-                        "autologging"
+                        "autologging",
+                        "PyYAML"
                     ],
       python_requires='>=3.0',
       )
-
-
-
```

