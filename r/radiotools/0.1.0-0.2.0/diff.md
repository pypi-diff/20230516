# Comparing `tmp/radiotools-0.1.0.tar.gz` & `tmp/radiotools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiotools-0.1.0.tar", last modified: Thu May 30 23:03:12 2019, max compression
+gzip compressed data, was "radiotools-0.2.0.tar", last modified: Thu Sep  5 17:09:24 2019, max compression
```

## Comparing `radiotools-0.1.0.tar` & `radiotools-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1319 2019-05-30 23:02:45.542960 radiotools-0.1.0/.gitignore
--rw-r--r--   0        0        0    35141 2017-10-11 17:24:05.294484 radiotools-0.1.0/LICENSE
--rw-r--r--   0        0        0      138 2019-01-11 23:14:37.579594 radiotools-0.1.0/README.md
--rw-r--r--   0        0        0      320 2019-05-30 22:59:04.172618 radiotools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       90 2019-05-30 22:50:57.027172 radiotools-0.1.0/radiotools/__init__.py
--rw-r--r--   0        0        0        0 2017-11-23 00:35:35.645262 radiotools-0.1.0/radiotools/analyses/__init__.py
--rw-r--r--   0        0        0     3681 2019-01-11 23:14:37.579855 radiotools-0.1.0/radiotools/analyses/energy_fluence.py
--rw-r--r--   0        0        0     3415 2017-12-11 22:29:48.652379 radiotools-0.1.0/radiotools/analyses/radiationenergy.py
--rw-r--r--   0        0        0        0 2017-11-23 00:37:00.811930 radiotools-0.1.0/radiotools/atmosphere/__init__.py
--rw-r--r--   0        0        0    56695 2019-01-24 19:40:07.273239 radiotools-0.1.0/radiotools/atmosphere/models.py
--rw-r--r--   0        0        0    10940 2019-05-30 22:42:55.835172 radiotools-0.1.0/radiotools/coordinatesystems.py
--rw-r--r--   0        0        0      623 2018-02-26 23:13:03.049901 radiotools-0.1.0/radiotools/coreas/GE.py
--rw-r--r--   0        0        0     1482 2018-02-26 21:50:57.383712 radiotools-0.1.0/radiotools/coreas/LSF.py
--rw-r--r--   0        0        0        0 2018-02-26 21:50:50.949844 radiotools-0.1.0/radiotools/coreas/__init__.py
--rw-r--r--   0        0        0    19058 2018-02-28 02:53:46.414002 radiotools-0.1.0/radiotools/coreas/generate_coreas_sim.py
--rw-r--r--   0        0        0     4875 2018-02-26 22:40:25.881389 radiotools-0.1.0/radiotools/coreas/geninp_aera.py
--rw-r--r--   0        0        0      608 2018-12-20 10:11:49.887703 radiotools-0.1.0/radiotools/doc/Makefile
--rw-r--r--   0        0        0      305 2017-12-11 22:18:55.883014 radiotools-0.1.0/radiotools/doc/analyses.rst
--rw-r--r--   0        0        0     5316 2017-12-11 20:48:46.419712 radiotools-0.1.0/radiotools/doc/conf.py
--rw-r--r--   0        0        0      146 2017-12-11 21:03:33.222085 radiotools-0.1.0/radiotools/doc/coordinatesystems.rst
--rw-r--r--   0        0        0       85 2017-12-11 20:43:07.361264 radiotools-0.1.0/radiotools/doc/helper.rst
--rw-r--r--   0        0        0     1035 2017-12-11 22:15:52.075272 radiotools-0.1.0/radiotools/doc/index.rst
--rw-r--r--   0        0        0       86 2017-12-11 20:42:57.541313 radiotools-0.1.0/radiotools/doc/plthelpers.rst
--rw-r--r--   0        0        0    28262 2019-05-30 22:42:55.835777 radiotools-0.1.0/radiotools/helper.py
--rw-r--r--   0        0        0    10436 2016-11-25 15:11:33.000000 radiotools-0.1.0/radiotools/leapseconds.py
--rw-r--r--   0        0        0    17305 2019-05-30 22:42:55.836180 radiotools-0.1.0/radiotools/plthelpers.py
--rw-r--r--   0        0        0     5200 2018-08-21 22:02:02.832794 radiotools-0.1.0/radiotools/stats.py
--rw-r--r--   0        0        0    24470 2019-05-30 22:42:55.837574 radiotools-0.1.0/tests/test_data/efield_traces.npz
--rw-r--r--   0        0        0      944 2019-05-30 22:42:55.838280 radiotools-0.1.0/tests/tests_atmosphere.py
--rw-r--r--   0        0        0     2366 2019-05-30 22:42:55.838978 radiotools-0.1.0/tests/tests_coordinatesystems.py
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 radiotools-0.1.0/setup.py
--rw-r--r--   0        0        0      229 1970-01-01 00:00:00.000000 radiotools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1338 2019-09-05 16:58:54.242863 radiotools-0.2.0/.gitignore
+-rw-r--r--   0        0        0      239 2019-09-05 16:58:54.243032 radiotools-0.2.0/.travis.yml
+-rw-r--r--   0        0        0    35141 2019-09-05 16:58:54.243400 radiotools-0.2.0/LICENSE
+-rw-r--r--   0        0        0      138 2019-09-05 16:58:54.243519 radiotools-0.2.0/README.md
+-rw-r--r--   0        0        0      343 2019-09-05 17:09:22.571998 radiotools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       91 2019-09-05 16:59:10.355057 radiotools-0.2.0/radiotools/__init__.py
+-rw-r--r--   0        0        0        0 2019-09-05 16:58:54.243948 radiotools-0.2.0/radiotools/analyses/__init__.py
+-rw-r--r--   0        0        0     3681 2019-09-05 16:58:54.244086 radiotools-0.2.0/radiotools/analyses/energy_fluence.py
+-rw-r--r--   0        0        0     3415 2019-09-05 16:58:54.244239 radiotools-0.2.0/radiotools/analyses/radiationenergy.py
+-rw-r--r--   0        0        0        0 2019-09-05 16:58:54.244370 radiotools-0.2.0/radiotools/atmosphere/__init__.py
+-rw-r--r--   0        0        0    40464 2019-09-05 16:58:54.244746 radiotools-0.2.0/radiotools/atmosphere/models.py
+-rw-r--r--   0        0        0    10940 2019-09-05 16:58:54.244912 radiotools-0.2.0/radiotools/coordinatesystems.py
+-rw-r--r--   0        0        0      623 2019-09-05 16:58:54.245124 radiotools-0.2.0/radiotools/coreas/GE.py
+-rw-r--r--   0        0        0     1482 2019-09-05 16:58:54.245253 radiotools-0.2.0/radiotools/coreas/LSF.py
+-rw-r--r--   0        0        0        0 2019-09-05 16:58:54.245340 radiotools-0.2.0/radiotools/coreas/__init__.py
+-rw-r--r--   0        0        0    19091 2019-09-05 16:58:54.245504 radiotools-0.2.0/radiotools/coreas/generate_coreas_sim.py
+-rw-r--r--   0        0        0     4875 2019-09-05 16:58:54.245837 radiotools-0.2.0/radiotools/coreas/geninp_aera.py
+-rw-r--r--   0        0        0      608 2019-09-05 16:58:54.246237 radiotools-0.2.0/radiotools/doc/Makefile
+-rw-r--r--   0        0        0      305 2019-09-05 16:58:54.246475 radiotools-0.2.0/radiotools/doc/analyses.rst
+-rw-r--r--   0        0        0     5316 2019-09-05 16:58:54.246672 radiotools-0.2.0/radiotools/doc/conf.py
+-rw-r--r--   0        0        0      146 2019-09-05 16:58:54.246827 radiotools-0.2.0/radiotools/doc/coordinatesystems.rst
+-rw-r--r--   0        0        0       85 2019-09-05 16:58:54.246988 radiotools-0.2.0/radiotools/doc/helper.rst
+-rw-r--r--   0        0        0     1035 2019-09-05 16:58:54.247115 radiotools-0.2.0/radiotools/doc/index.rst
+-rw-r--r--   0        0        0       86 2019-09-05 16:58:54.247242 radiotools-0.2.0/radiotools/doc/plthelpers.rst
+-rw-r--r--   0        0        0    28713 2019-09-05 16:58:54.247846 radiotools-0.2.0/radiotools/helper.py
+-rw-r--r--   0        0        0    10436 2019-09-05 16:58:54.248047 radiotools-0.2.0/radiotools/leapseconds.py
+-rw-r--r--   0        0        0    17372 2019-09-05 16:58:54.248264 radiotools-0.2.0/radiotools/plthelpers.py
+-rw-r--r--   0        0        0     5200 2019-09-05 16:58:54.248406 radiotools-0.2.0/radiotools/stats.py
+-rw-r--r--   0        0        0    24470 2019-09-05 16:58:54.248798 radiotools-0.2.0/tests/test_data/efield_traces.npz
+-rw-r--r--   0        0        0    15312 2019-09-05 16:58:54.248994 radiotools-0.2.0/tests/tests_atmosphere.py
+-rw-r--r--   0        0        0     2370 2019-09-05 16:58:54.249140 radiotools-0.2.0/tests/tests_coordinatesystems.py
+-rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 radiotools-0.2.0/setup.py
+-rw-r--r--   0        0        0      229 1970-01-01 00:00:00.000000 radiotools-0.2.0/PKG-INFO
```

### Comparing `radiotools-0.1.0/.gitignore` & `radiotools-0.2.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 
+# atmosphere files
 radiotools/atmosphere/constants*
 
 .project
 .pydevproject
 .settings/
 radiotools/doc/_build/
 radiotools/doc/copy_docs_to_cglaserde.sh
```

### Comparing `radiotools-0.1.0/LICENSE` & `radiotools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/analyses/energy_fluence.py` & `radiotools-0.2.0/radiotools/analyses/energy_fluence.py`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/analyses/radiationenergy.py` & `radiotools-0.2.0/radiotools/analyses/radiationenergy.py`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/coordinatesystems.py` & `radiotools-0.2.0/radiotools/coordinatesystems.py`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/coreas/GE.py` & `radiotools-0.2.0/radiotools/coreas/GE.py`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/coreas/LSF.py` & `radiotools-0.2.0/radiotools/coreas/LSF.py`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/coreas/generate_coreas_sim.py` & `radiotools-0.2.0/radiotools/coreas/generate_coreas_sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import absolute_import, division, print_function  # , unicode_literals
 import os
 import stat
 import numpy as np
 from radiotools import coordinatesystems
 from radiotools import helper as hp
+from past.builtins import xrange
 
 
 # $_CONDOR_SCRATCH_DIR
 
 
 def write_sh_geninponly(filename, output_dir, run_dir, corsika_executable,
                          seed, particle_type, event_number, energy, zenith, azimuth,
```

### Comparing `radiotools-0.1.0/radiotools/coreas/geninp_aera.py` & `radiotools-0.2.0/radiotools/coreas/geninp_aera.py`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/doc/Makefile` & `radiotools-0.2.0/radiotools/doc/Makefile`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/doc/conf.py` & `radiotools-0.2.0/radiotools/doc/conf.py`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/doc/index.rst` & `radiotools-0.2.0/radiotools/doc/index.rst`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/helper.py` & `radiotools-0.2.0/radiotools/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, division, print_function  # , unicode_literals
-
 import numpy as np
 
 
 def linear_to_dB(linear):
     """ conversion to decibel scale
 
     Parameters
@@ -66,15 +65,15 @@
 
 def spherical_to_cartesian(zenith, azimuth):
     sinZenith = np.sin(zenith)
     x = sinZenith * np.cos(azimuth)
     y = sinZenith * np.sin(azimuth)
     z = np.cos(zenith)
     if hasattr(zenith, '__len__') and hasattr(azimuth, '__len__'):
-        return np.array(zip(x, y, z))
+        return np.array([x, y, z]).T
     else:
         return np.array([x, y, z])
 
 
 def cartesian_to_spherical(x, y, z):
     # normlize vector
     norm = (x ** 2 + y ** 2 + z ** 2) ** 0.5
@@ -235,15 +234,15 @@
 def get_interval(trace, scale=0.5):
     h = np.abs(trace)
     max_pos = h.argmax()
     n_samples = trace.T.shape[0]
     h_max = h.max()
     up_pos = max_pos
     low_pos = max_pos
-    for i in xrange(max_pos, n_samples):
+    for i in range(max_pos, n_samples):
         if (h[i] < h_max * scale):
             up_pos = i
             break
     for i in range(0, max_pos)[::-1]:
         if (h[i] < h_max * scale):
             low_pos = i
             break
@@ -316,15 +315,15 @@
     cs = CSTransformation(zenith, azimuth)
     efield_transformed = cs.transform_to_vxB_vxvxB(efield)
     #     print "efieldtransformed ", efield_transformed
     if (len(stationPositions.shape) == 1):
         if (efield_transformed[0] > 0):
             efield_transformed *= -1.
     else:
-        for i in xrange(len(efield_transformed)):
+        for i in range(len(efield_transformed)):
             if (efield_transformed[i][0] > 0):
                 efield_transformed[i] *= -1.
 
     efield_expectations = get_expected_efield_vector(core, zenith, azimuth,
                                                      stationPositions, a=a,
                                                      magnetic_field_vector=magnetic_field_vector)
     exp_efields_transformed = cs.transform_to_vxB_vxvxB(efield_expectations)
@@ -337,15 +336,15 @@
     diff = exp_phi - phi
     if (len(stationPositions.shape) == 1):
         while (diff > np.pi):
             diff -= 2 * np.pi
         while (diff < -np.pi):
             diff += 2 * np.pi
     else:
-        for i in xrange(len(diff)):
+        for i in range(len(diff)):
             while (diff[i] > np.pi):
                 diff[i] -= 2 * np.pi
             while (diff[i] < -np.pi):
                 diff[i] += 2 * np.pi
     return diff
 
 
@@ -679,14 +678,28 @@
   
     # calculating regression coefficients 
     b = SS_xy / SS_xx  # slope 
     a = m_y - b * m_x  # zero-offset
   
     return(a, b) 
 
+def pretty_time_delta(seconds):
+    seconds = int(seconds)
+    days, seconds = divmod(seconds, 86400)
+    hours, seconds = divmod(seconds, 3600)
+    minutes, seconds = divmod(seconds, 60)
+    if days > 0:
+        return '%dd%dh%dm%ds' % (days, hours, minutes, seconds)
+    elif hours > 0:
+        return '%dh%dm%ds' % (hours, minutes, seconds)
+    elif minutes > 0:
+        return '%dm%ds' % (minutes, seconds)
+    else:
+        return '%ds' % (seconds,)
+
 
 # Test Code:
 if __name__ == "__main__":
 
     import radiotools.HelperFunctions as hp
 
     n = 10000
```

### Comparing `radiotools-0.1.0/radiotools/leapseconds.py` & `radiotools-0.2.0/radiotools/leapseconds.py`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/radiotools/plthelpers.py` & `radiotools-0.2.0/radiotools/plthelpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import inspect, re
 import math
 import os
 from matplotlib import colors as mcolors
+from past.builtins import xrange
 
 from scipy import optimize
 
 import matplotlib.pyplot as plt
 import numpy as np
+import radiotools.stats
 
 
 def get_discrete_cmap(N, base_cmap='viridis'):
     cmap = plt.get_cmap(base_cmap, N)
     colors = []
     N = np.int(N)
     for i in range(N):
@@ -165,37 +167,35 @@
                 textstr += "$\mu = {:.3g}$\n".format(tmean)
             else:
                 textstr += "$\mu = {:.3g}$\n".format(tmean)
         if median:
             tweights = np.ones_like(data)
             if weights is not None:
                 tweights = weights
-            import stats
             if quantiles:
-                q1 = stats.quantile_1d(data, tweights, 0.16)
-                q2 = stats.quantile_1d(data, tweights, 0.84)
-                median = stats.median(data, tweights)
+                q1 = radiotools.stats.quantile_1d(data, tweights, 0.16)
+                q2 = radiotools.stats.quantile_1d(data, tweights, 0.84)
+                median = radiotools.stats.median(data, tweights)
     #             median_str = serror.formatError(median, 0.05 * (np.abs(median - q2) + np.abs(median - q1)))[0]
                 textstr += "$\mathrm{median} = %.3g^{+%.2g}_{-%.2g}$\n" % (median, np.abs(median - q2),
                                                                            np.abs(median - q1))
             else:
-                textstr += "$\mathrm{median} = %.3g $\n" % stats.median(data, tweights)
+                textstr += "$\mathrm{median} = %.3g $\n" % radiotools.stats.median(data, tweights)
         if std:
             if rel:
                 textstr += "$\sigma = %.2g$ (%.1f\%%)\n" % (tstd, tstd / tmean * 100.)
             else:
                 textstr += "$\sigma = %.2g$\n" % (tstd)
     else:
-        import stat
         if(weights is None):
             w = np.ones_like(data)
         else:
             w = weights
-        q68 = stats.quantile_1d(data, weights=w, quant=.68)
-        q95 = stats.quantile_1d(data, weights=w, quant=.95)
+        q68 = radiotools.stats.quantile_1d(data, weights=w, quant=.68)
+        q95 = radiotools.stats.quantile_1d(data, weights=w, quant=.95)
         textstr += "$\sigma_\mathrm{{68}}$ = {:.1f}$^\circ$\n".format(q68)
         textstr += "$\sigma_\mathrm{{95}}$ = {:.1f}$^\circ$\n".format(q95)
 
     if(overflow):
         textstr += "$\mathrm{overflows} = %i$\n" % overflow
     if(underflow):
         textstr += "$\mathrm{underflows} = %i$\n" % underflow
@@ -374,15 +374,15 @@
             fig, ax1 = plt.subplots(1, 1, figsize=figsize)
     else:
         ax1 = ax
 
     ax1.set_xlabel(xlabel)
     ax1.set_ylabel(ylabel)
     ax1.set_title(title)
-    n, bins, patches = ax1.hist(data, bins, density=0, weights=weights, **kwargs)
+    n, bins, patches = ax1.hist(data, bins, weights=weights, **kwargs)
     if(funcs):
         for func in funcs:
             xlim = np.array(ax1.get_xlim())
             xx = np.linspace(xlim[0], xlim[1], 100)
             if('args' in func):
                 ax1.plot(xx, func['func'](xx), *func['args'])
                 if('kwargs' in func):
```

### Comparing `radiotools-0.1.0/radiotools/stats.py` & `radiotools-0.2.0/radiotools/stats.py`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/tests/test_data/efield_traces.npz` & `radiotools-0.2.0/tests/test_data/efield_traces.npz`

 * *Files identical despite different names*

### Comparing `radiotools-0.1.0/tests/tests_coordinatesystems.py` & `radiotools-0.2.0/tests/tests_coordinatesystems.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 v_xyz = -1 * np.array([np.sin(zenith) * np.cos(azimuth),
                        np.sin(zenith) * np.sin(azimuth),
                        np.cos(zenith)])
 
 v_vB_vvB2 = np.array([v_vB_vvB, 2 * v_vB_vvB])
 
 # test traces
-test_data = np.load("./test_data/efield_traces.npz", "r")
+test_data = np.load("tests/test_data/efield_traces.npz", "r")
 t_xyz = test_data["t_xyz"]
 t_vB_vvB = test_data["t_vBvvB"]
 
 
 class CoordinateTests(unittest.TestCase):
 
     def test_constant_input(self):
```

