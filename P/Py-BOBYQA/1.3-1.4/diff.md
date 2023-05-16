# Comparing `tmp/Py-BOBYQA-1.3.tar.gz` & `tmp/Py-BOBYQA-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Py-BOBYQA-1.3.tar", last modified: Wed Apr 14 00:46:30 2021, max compression
+gzip compressed data, was "dist/Py-BOBYQA-1.4.tar", last modified: Tue May 16 02:37:47 2023, max compression
```

## Comparing `Py-BOBYQA-1.3.tar` & `Py-BOBYQA-1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 lindon    (1000) lindon    (1000)        0 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     9410 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/PKG-INFO
-drwxrwxrwx   0 lindon    (1000) lindon    (1000)        0 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/pybobyqa/
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    30336 2020-04-20 01:52:14.000000 Py-BOBYQA-1.3/pybobyqa/controller.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     5958 2020-04-20 01:52:14.000000 Py-BOBYQA-1.3/pybobyqa/diagnostic_info.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     4352 2021-02-25 02:56:44.000000 Py-BOBYQA-1.3/pybobyqa/hessian.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    19906 2021-04-14 00:25:18.000000 Py-BOBYQA-1.3/pybobyqa/model.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    12892 2020-04-20 01:52:14.000000 Py-BOBYQA-1.3/pybobyqa/params.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    48810 2021-02-25 02:57:05.000000 Py-BOBYQA-1.3/pybobyqa/solver.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    15868 2021-04-14 00:25:24.000000 Py-BOBYQA-1.3/pybobyqa/trust_region.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     8599 2020-04-20 01:52:14.000000 Py-BOBYQA-1.3/pybobyqa/util.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)      924 2021-04-14 00:35:12.000000 Py-BOBYQA-1.3/pybobyqa/version.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     1562 2020-04-20 01:52:14.000000 Py-BOBYQA-1.3/pybobyqa/__init__.py
-drwxrwxrwx   0 lindon    (1000) lindon    (1000)        0 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/Py_BOBYQA.egg-info/
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)        1 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/Py_BOBYQA.egg-info/dependency_links.txt
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     9410 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/Py_BOBYQA.egg-info/PKG-INFO
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)       69 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/Py_BOBYQA.egg-info/requires.txt
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)      421 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/Py_BOBYQA.egg-info/SOURCES.txt
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)        9 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/Py_BOBYQA.egg-info/top_level.txt
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)        1 2020-04-21 23:25:10.000000 Py-BOBYQA-1.3/Py_BOBYQA.egg-info/zip-safe
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     6945 2021-04-14 00:46:05.000000 Py-BOBYQA-1.3/README.rst
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)       38 2021-04-14 00:46:30.000000 Py-BOBYQA-1.3/setup.cfg
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     2735 2021-04-14 00:35:58.000000 Py-BOBYQA-1.3/setup.py
+drwxrwxrwx   0 lindon    (1000) lindon    (1000)        0 2023-05-16 02:39:14.000000 Py-BOBYQA-1.4/
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)     9704 2023-05-16 02:39:14.000000 Py-BOBYQA-1.4/PKG-INFO
+drwxrwxrwx   0 lindon    (1000) lindon    (1000)        0 2023-05-16 02:39:14.000000 Py-BOBYQA-1.4/pybobyqa/
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)    31506 2021-11-10 06:40:49.000000 Py-BOBYQA-1.4/pybobyqa/controller.py
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)     6179 2021-04-14 00:51:00.000000 Py-BOBYQA-1.4/pybobyqa/diagnostic_info.py
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)     4352 2021-02-25 02:56:44.000000 Py-BOBYQA-1.4/pybobyqa/hessian.py
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)    19959 2021-11-03 06:24:10.000000 Py-BOBYQA-1.4/pybobyqa/model.py
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)    12892 2020-04-20 01:52:14.000000 Py-BOBYQA-1.4/pybobyqa/params.py
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)    49042 2021-11-03 06:32:05.000000 Py-BOBYQA-1.4/pybobyqa/solver.py
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)    16009 2021-10-11 06:29:48.000000 Py-BOBYQA-1.4/pybobyqa/trust_region.py
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)     8657 2021-11-03 06:24:53.000000 Py-BOBYQA-1.4/pybobyqa/util.py
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)      924 2023-05-16 02:28:16.000000 Py-BOBYQA-1.4/pybobyqa/version.py
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)     1562 2020-04-20 01:52:14.000000 Py-BOBYQA-1.4/pybobyqa/__init__.py
+drwxrwxrwx   0 lindon    (1000) lindon    (1000)        0 2023-05-16 02:39:13.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)        1 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/dependency_links.txt
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)     9704 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/PKG-INFO
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)       69 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/requires.txt
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)      421 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/SOURCES.txt
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)        9 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/top_level.txt
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)        1 2020-04-21 23:25:10.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/zip-safe
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)     7208 2021-12-09 02:59:49.000000 Py-BOBYQA-1.4/README.rst
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)       38 2023-05-16 02:39:14.000000 Py-BOBYQA-1.4/setup.cfg
+-rwxrwxrwx   0 lindon    (1000) lindon    (1000)     2734 2023-05-16 02:30:14.000000 Py-BOBYQA-1.4/setup.py
```

### Comparing `Py-BOBYQA-1.3/PKG-INFO` & `Py-BOBYQA-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: Py-BOBYQA
-Version: 1.3
+Version: 1.4
 Summary: A flexible derivative-free solver for (bound constrained) general objective minimization
 Home-page: https://github.com/numericalalgorithmsgroup/pybobyqa/
 Author: Lindon Roberts
-Author-email: lindon.roberts@maths.ox.ac.uk
+Author-email: lindon.roberts@sydney.edu.au
 License: GNU GPL
-Download-URL: https://github.com/numericalalgorithmsgroup/pybobyqa/archive/v1.3.tar.gz
+Download-URL: https://github.com/numericalalgorithmsgroup/pybobyqa/archive/v1.4.tar.gz
 Description: ====================================================================
         Py-BOBYQA: Derivative-Free Solver for Bound-Constrained Minimization
         ====================================================================
         
-        .. image::  https://travis-ci.org/numericalalgorithmsgroup/pybobyqa.svg?branch=master
-           :target: https://travis-ci.org/numericalalgorithmsgroup/pybobyqa
+        .. image::  https://github.com/numericalalgorithmsgroup/pybobyqa/actions/workflows/python_testing.yml/badge.svg
+           :target: https://github.com/numericalalgorithmsgroup/pybobyqa/actions
            :alt: Build Status
         
         .. image::  https://img.shields.io/badge/License-GPL%20v3-blue.svg
            :target: https://www.gnu.org/licenses/gpl-3.0
            :alt: GNU GPL v3 License
         
         .. image:: https://img.shields.io/pypi/v/Py-BOBYQA.svg
            :target: https://pypi.python.org/pypi/Py-BOBYQA
            :alt: Latest PyPI version
         
         .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2630437.svg
            :target: https://doi.org/10.5281/zenodo.2630437
            :alt: DOI:10.5281/zenodo.2630437
         
+        .. image:: https://static.pepy.tech/personalized-badge/py-bobyqa?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads
+         :target: https://pepy.tech/project/py-bobyqa
+           :alt: Total downloads
+        
         Py-BOBYQA is a flexible package for solving bound-constrained general objective minimization, without requiring derivatives of the objective. At its core, it is a Python implementation of the BOBYQA algorithm by Powell, but Py-BOBYQA has extra features improving its performance on some problems (see the papers below for details). Py-BOBYQA is particularly useful when evaluations of the objective function are expensive and/or noisy.
         
         More details about Py-BOBYQA and its enhancements over BOBYQA can be found in our papers:
         
         1. Coralia Cartis, Jan Fiala, Benjamin Marteau and Lindon Roberts, `Improving the Flexibility and Robustness of Model-Based Derivative-Free Optimization Solvers <https://doi.org/10.1145/3338517>`_, *ACM Transactions on Mathematical Software*, 45:3 (2019), pp. 32:1-32:41 [`arXiv preprint: 1804.00154 <https://arxiv.org/abs/1804.00154>`_] 
         2. Coralia Cartis, Lindon Roberts and Oliver Sheridan-Methven, `Escaping local minima with derivative-free methods: a numerical investigation <https://doi.org/10.1080/02331934.2021.1883015>`_, *Optimization* (2021). [`arXiv preprint: 1812.11343 <https://arxiv.org/abs/1812.11343>`_]
```

### Comparing `Py-BOBYQA-1.3/pybobyqa/controller.py` & `Py-BOBYQA-1.4/pybobyqa/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 from .trust_region import *
 from .util import *
 
 __all__ = ['Controller', 'ExitInformation', 'EXIT_SLOW_WARNING', 'EXIT_MAXFUN_WARNING', 'EXIT_SUCCESS',
            'EXIT_INPUT_ERROR', 'EXIT_TR_INCREASE_ERROR', 'EXIT_LINALG_ERROR', 'EXIT_FALSE_SUCCESS_WARNING',
            'EXIT_AUTO_DETECT_RESTART_WARNING']
 
+module_logger = logging.getLogger(__name__) 
+
 EXIT_AUTO_DETECT_RESTART_WARNING = 4  # warning, auto-detected restart criteria
 EXIT_FALSE_SUCCESS_WARNING = 3  # warning, maximum fake successful steps reached
 EXIT_SLOW_WARNING = 2  # warning, maximum number of slow (successful) iterations reached
 EXIT_MAXFUN_WARNING = 1  # warning, reached max function evals
 EXIT_SUCCESS = 0  # successful finish (rho=rhoend, sufficient objective reduction, or everything in noise level)
 EXIT_INPUT_ERROR = -1  # error, bad inputs
 EXIT_TR_INCREASE_ERROR = -2  # error, trust region step increased model value
@@ -127,15 +129,15 @@
         return self.model.n()
 
     def npt(self):
         return self.model.npt()
 
     def initialise_coordinate_directions(self, number_of_samples, num_directions, params):
         if self.do_logging:
-            logging.debug("Initialising with coordinate directions")
+            module_logger.debug("Initialising with coordinate directions")
         # self.model already has x0 evaluated, so only need to initialise the other points
         # num_directions = params("growing.ndirs_initial")
         assert self.model.num_pts <= (self.n() + 1) * (self.n() + 2) // 2, "prelim: must have npt <= (n+1)(n+2)/2"
         assert 1 <= num_directions < self.model.num_pts, "Initialisation: must have 1 <= ndirs_initial < npt"
 
         at_lower_boundary = (self.model.sl > -0.01 * self.delta)  # sl = xl - x0, should be -ve, actually < -rhobeg
         at_upper_boundary = (self.model.su < 0.01 * self.delta)  # su = xu - x0, should be +ve, actually > rhobeg
@@ -201,15 +203,15 @@
                 if stepa * stepb < 0.0 and self.model.fval(k) < self.model.fval(k - self.n()):
                     xpts_added[[k, k-self.n()]] = xpts_added[[k-self.n(), k]]
 
         return None   # return & continue
 
     def initialise_random_directions(self, number_of_samples, num_directions, params):
         if self.do_logging:
-            logging.debug("Initialising with random orthogonal directions")
+            module_logger.debug("Initialising with random orthogonal directions")
         # self.model already has x0 evaluated, so only need to initialise the other points
         # num_directions = params("growing.ndirs_initial")
         assert 1 <= num_directions < self.model.num_pts, "Initialisation: must have 1 <= ndirs_initial < npt"
 
         # Get ndirs_initial random orthogonal directions
         xopt = self.model.xopt()
         if params("init.random_directions_make_orthogonal"):
@@ -265,27 +267,42 @@
                     self.model.add_new_sample(1 + ndirns, f_extra=f_list[i])
 
         return None
 
     def trust_region_step(self):
         # Build model for full least squares objectives
         gopt, H = self.model.build_full_model()
-        d, gnew, crvmin = trsbox(self.model.xopt(), gopt, H, self.model.sl, self.model.su, self.delta)
+        try:
+            d, gnew, crvmin = trsbox(self.model.xopt(), gopt, H, self.model.sl, self.model.su, self.delta)
+        except ValueError:
+            # A ValueError may be raised if gopt or H have nan/inf values (issue #14)
+            # Although this should be picked up earlier, in this situation just return a zero 
+            # trust-region step, which leads to a safety step being called in the main algorithm.
+            d = np.zeros(gopt.shape)
+            gnew = gopt.copy()
+            crvmin = 0.0  # this usually represents 'step on trust-region boundary' but seems to be a sensible default for errors
         return d, gopt, H, gnew, crvmin
 
     def geometry_step(self, knew, adelt, number_of_samples, params):
         if self.do_logging:
-            logging.debug("Running geometry-fixing step")
+            module_logger.debug("Running geometry-fixing step")
         try:
             c, g, H = self.model.lagrange_polynomial(knew)  # based at xopt
-            # Solve problem: bounds are sl <= xnew <= su, and ||xnew-xopt|| <= adelt
-            xnew = trsbox_geometry(self.model.xopt(), c, g, H, self.model.sl, self.model.su, adelt)
         except LA.LinAlgError:
             exit_info = ExitInformation(EXIT_LINALG_ERROR, "Singular matrix encountered in geometry step")
             return exit_info  # didn't fix geometry - return & quit
+        
+        # Solve problem: bounds are sl <= xnew <= su, and ||xnew-xopt|| <= adelt
+        try:
+            xnew = trsbox_geometry(self.model.xopt(), c, g, H, self.model.sl, self.model.su, adelt)
+        except ValueError:
+            # A ValueError may be raised if gopt or H have nan/inf values (issue #23)
+            # Ideally this should be picked up earlier in self.model.lagrange_polynomial(...)
+            exit_info = ExitInformation(EXIT_LINALG_ERROR, "Error when calculating geometry-improving step")
+            return exit_info  # didn't fix geometry - return & quit
 
         gopt, H = self.model.build_full_model()  # save here, to calculate predicted value from geometry step
         fopt = self.model.fopt()  # again, evaluate now, before model.change_point()
         d = xnew - self.model.xopt()
         x = self.model.as_absolute_coordinates(xnew)
         f_list, num_samples_run, exit_info = self.evaluate_objective(x, number_of_samples, params)
 
@@ -455,20 +472,20 @@
             self.last_fopts_step_taken = self.last_fopts_step_taken[1:] + [self.model.fopt()]
             this_iter_slow = (self.last_fopts_step_taken[0] - self.model.fopt()) / \
                          float(params("slow.history_for_slow")) < params("slow.thresh_for_slow")
         # Update counter of number of slow iterations
         if this_iter_slow:
             self.num_slow_iters += 1
             if self.do_logging:
-                logging.info("Slow iteration (%g consecutive so far, max allowed %g)"
+                module_logger.info("Slow iteration (%g consecutive so far, max allowed %g)"
                          % (self.num_slow_iters, params("slow.max_slow_iters")))
         else:
             self.num_slow_iters = 0
             if self.do_logging:
-                logging.debug("Non-slow iteration")
+                module_logger.debug("Non-slow iteration")
         return this_iter_slow, self.num_slow_iters >= params("slow.max_slow_iters")
 
     def soft_restart(self, number_of_samples, nruns_so_far, params, x_in_abs_coords_to_save=None, f_to_save=None,
                      nsamples_to_save=None):
         # A successful run is one where we reduced fopt
         if self.model.fopt() < self.last_run_fopt:
             self.last_successful_run = nruns_so_far
@@ -495,20 +512,25 @@
             assert f_to_save is not None, "Soft restart: specified x_to_save but not rvec_to_save"
             assert nsamples_to_save is not None, "Soft restart: specified x_to_save but not nsamples_to_save"
             self.model.save_point(x_in_abs_coords_to_save, f_to_save, nsamples_to_save, x_in_abs_coords=True)
         self.model.save_point(self.model.xopt(abs_coordinates=True), self.model.fopt(),
                               self.model.nsamples[self.model.kopt], x_in_abs_coords=True)
 
         if self.do_logging:
-            logging.info("Soft restart [currently, f = %g after %g function evals]" % (self.model.fopt(), self.nf))
+            module_logger.info("Soft restart [currently, f = %g after %g function evals]" % (self.model.fopt(), self.nf))
         # Resetting method: reset delta and rho, then move the closest 'num_steps' points to xk to improve geometry
         # Note: closest points because we are suddenly increasing delta & rho, so we want to encourage spreading out points
         self.delta = self.rhobeg
         self.rho = self.rhobeg
         self.diffs = [0.0, 0.0, 0.0]
+        
+        # Forget history of slow iterations
+        self.last_iters_step_taken = []
+        self.last_fopts_step_taken = []
+        self.num_slow_iters = 0
 
         all_sq_dist = self.model.distances_to_xopt()[:self.model.npt()]
         closest_points = np.argsort(all_sq_dist)
         if params("restarts.soft.move_xk"):
             closest_points = closest_points[:params("restarts.soft.num_geom_steps")]
             upper_limit = self.model.num_pts
         else:
```

### Comparing `Py-BOBYQA-1.3/pybobyqa/diagnostic_info.py` & `Py-BOBYQA-1.4/pybobyqa/diagnostic_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,20 @@
 
 """
 
 # Ensure compatibility with Python 2
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import numpy as np
-import pandas as pd
+try:
+    import pandas as pd
+    HAVE_PANDAS = True
+except ImportError:
+    # If pandas not available, return diagnostic info as a Python dict
+    HAVE_PANDAS = False
 from .util import remove_scaling
 
 
 __all__ = ['DiagnosticInfo', 'ITER_VERY_SUCCESSFUL', 'ITER_SUCCESSFUL', 'ITER_ACCEPTABLE_GEOM',
            'ITER_ACCEPTABLE_NO_GEOM', 'ITER_UNSUCCESSFUL_GEOM', 'ITER_UNSUCCESSFUL_NO_GEOM', 'ITER_SAFETY']
 
 
@@ -80,15 +85,18 @@
 
     def to_dataframe(self, with_xk=False):
         data_to_save = {}
         for key in self.data:
             if key == "xk" and not with_xk:
                 continue  # skip
             data_to_save[key] = self.data[key]
-        return pd.DataFrame(data_to_save)
+        if HAVE_PANDAS:
+            return pd.DataFrame(data_to_save)
+        else:
+            return data_to_save
 
     def to_csv(self, filename):
         df = self.to_dataframe()
         df.to_csv(filename)
 
     def save_info_from_control(self, control, nruns, iter_this_run, save_poisedness=True):
         self.data["iters_total"].append(len(self.data["iters_total"]))
```

### Comparing `Py-BOBYQA-1.3/pybobyqa/hessian.py` & `Py-BOBYQA-1.4/pybobyqa/hessian.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.3/pybobyqa/model.py` & `Py-BOBYQA-1.4/pybobyqa/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 from .hessian import to_upper_triangular_vector
 from .trust_region import trsbox_geometry
 from .util import sumsq, model_value
 
 __all__ = ['Model']
 
 
+module_logger = logging.getLogger(__name__) 
+
+
 class Model(object):
     def __init__(self, npt, x0, f0, xl, xu, f0_nsamples, n=None, abs_tol=-1e20, precondition=True, do_logging=True):
         if n is None:
             n = len(x0)
         assert npt >= n + 1, "Require npt >= n+1 for quadratic models"
         assert npt <= (n+1)*(n + 2)//2, "Require npt <= (n+1)(n+2)/2 for quadratic models"
         assert x0.shape == (n,), "x0 has wrong shape (got %s, expect (%g,))" % (str(x0.shape), n)
@@ -256,15 +259,15 @@
 
         if self.factorisation_current:
             # A(preconditioned) = diag(left_scaling) * A(original) * diag(right_scaling)
             # Solve A(original)\rhs
             return col_scale(LA.lu_solve((self.lu, self.piv), col_scale(rhs, self.left_scaling)), self.right_scaling)
         else:
             if self.do_logging:
-                logging.warning("model.solve_system not using factorisation")
+                module_logger.warning("model.solve_system not using factorisation")
             A, left_scaling, right_scaling = self.interpolation_matrix()
             return col_scale(LA.solve(A, col_scale(rhs, left_scaling)), right_scaling)
 
     def interpolate_model(self, verbose=False, min_chg_hess=True, get_norm_model_chg=False):
         if verbose:
             A, left_scaling, right_scaling = self.interpolation_matrix()
             interp_cond_num = np.linalg.cond(A)  # scipy.linalg does not have condition number!
```

### Comparing `Py-BOBYQA-1.3/pybobyqa/params.py` & `Py-BOBYQA-1.4/pybobyqa/params.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.3/pybobyqa/solver.py` & `Py-BOBYQA-1.4/pybobyqa/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 from .controller import *
 from .diagnostic_info import *
 from .params import *
 from .util import *
 
 __all__ = ['solve']
 
+module_logger = logging.getLogger(__name__) 
+
 
 # A container for the results of the optimization routine
 class OptimResults(object):
     def __init__(self, xmin, fmin, gradmin, hessmin, nf, nx, nruns, exit_flag, exit_msg):
         self.x = xmin
         self.f = fmin
         self.gradient = gradmin
@@ -145,19 +147,19 @@
     control = Controller(objfun, x0, args, f0_avg, num_samples_run, xl, xu, npt, rhobeg, rhoend, nf, nx, maxfun, params, scaling_changes, do_logging=do_logging)
 
     # Initialise interpolation set
     number_of_samples = max(nsamples(control.delta, control.rho, 0, nruns_so_far), 1)
     num_directions = npt - 1
     if params("init.random_initial_directions"):
         if do_logging:
-            logging.info("Initialising (random directions)")
+            module_logger.info("Initialising (random directions)")
         exit_info = control.initialise_random_directions(number_of_samples, num_directions, params)
     else:
         if do_logging:
-            logging.info("Initialising (coordinate directions)")
+            module_logger.info("Initialising (coordinate directions)")
         exit_info = control.initialise_coordinate_directions(number_of_samples, num_directions, params)
     if exit_info is not None:
         x, f, gradmin, hessmin, nsamples = control.model.get_final_results()
         return x, f, None, None, nsamples, control.nf, control.nx, nruns_so_far + 1, exit_info, diagnostic_info
 
     # Save list of last N successful steps: whether they failed to be an improvement over fsave
     succ_steps_not_improvement = [False]*params("restarts.soft.max_fake_successful_steps")
@@ -170,15 +172,15 @@
         restart_auto_detect_chg_hess = -1.0 * np.ones((params("restarts.auto_detect.history"),))
 
     #------------------------------------------
     # Begin main loop
     # ------------------------------------------
     current_iter = -1
     if do_logging:
-        logging.info("Beginning main loop")
+        module_logger.info("Beginning main loop")
     if print_progress:
         print("{:^5}{:^7}{:^10}{:^10}{:^10}{:^10}{:^7}".format("Run", "Iter", "Obj", "Grad", "Delta", "rho", "Evals"))
     while True:
         current_iter += 1
 
         # Noise level exit check
         if params("noise.quit_on_noise_level") and control.all_values_within_noise_level(params):
@@ -227,15 +229,15 @@
                 nruns_so_far += 1
                 break  # quit
 
 
         # Trust region step
         d, gopt, H, gnew, crvmin = control.trust_region_step()
         if do_logging:
-            logging.debug("Trust region step is d = " + str(d))
+            module_logger.debug("Trust region step is d = " + str(d))
         xnew = control.model.xopt() + d
         dnorm = min(LA.norm(d), control.delta)
 
         if print_progress:
             print("{:^5}{:^7}{:^10.2e}{:^10.2e}{:^10.2e}{:^10.2e}{:^7}".format(nruns_so_far + 1, current_iter + 1,
                                                                                control.model.fopt(),
                                                                                np.linalg.norm(gopt), control.delta,
@@ -246,15 +248,15 @@
                                                    save_poisedness=params("logging.save_poisedness"))
             diagnostic_info.update_interpolation_information(interp_error, interp_cond_num, norm_chg_grad,
                                                              norm_chg_hess, LA.norm(gopt), LA.norm(d))
 
         if dnorm < params("general.safety_step_thresh") * control.rho:
             # (start safety step)
             if do_logging:
-                logging.debug("Safety step (main phase)")
+                module_logger.debug("Safety step (main phase)")
 
             if params("logging.save_diagnostic_info"):
                 diagnostic_info.update_ratio(np.nan)
                 diagnostic_info.update_iter_type(ITER_SAFETY)
                 diagnostic_info.update_slow_iter(-1)
 
             if not control.done_with_current_rho(xnew, gnew, crvmin, H, current_iter):
@@ -291,20 +293,20 @@
                     continue  # next iteration
 
             # If we are done with the current rho, or didn't fix geometry above, reduce rho
             if control.rho > rhoend:
                 # Reduce rho
                 control.reduce_rho(current_iter, params)
                 if do_logging:
-                    logging.info("New rho = %g after %i function evaluations" % (control.rho, control.nf))
+                    module_logger.info("New rho = %g after %i function evaluations" % (control.rho, control.nf))
                     if control.n() < params("logging.n_to_print_whole_x_vector"):
-                        logging.debug("Best so far: f = %.15g at x = " % (control.model.fopt())
+                        module_logger.debug("Best so far: f = %.15g at x = " % (control.model.fopt())
                                       + str(control.model.xopt(abs_coordinates=True)))
                     else:
-                        logging.debug("Best so far: f = %.15g at x = [...]" % (control.model.fopt()))
+                        module_logger.debug("Best so far: f = %.15g at x = [...]" % (control.model.fopt()))
                 continue  # next iteration
             else:
                 # Quit on rho=rhoend
                 if params("restarts.use_restarts") and params("restarts.use_soft_restarts"):
                     number_of_samples = max(nsamples(control.delta, control.rho, current_iter, nruns_so_far), 1)
                     exit_info = control.soft_restart(number_of_samples, nruns_so_far, params,
                                          x_in_abs_coords_to_save=None, f_to_save=None, nsamples_to_save=None)
@@ -336,15 +338,15 @@
                     exit_info = ExitInformation(EXIT_SUCCESS, "rho has reached rhoend")
                     nruns_so_far += 1
                     break  # quit
             # (end safety step)
         else:
             # (start trust region step)
             if do_logging:
-                logging.debug("Standard trust region step")
+                module_logger.debug("Standard trust region step")
 
             # Add chgJ and delta to restart auto-detect set
             if params("restarts.use_restarts") and params("restarts.auto_detect"):
                 if restart_auto_detect_full:
                     # Drop first values, add new values at end
                     restart_auto_detect_delta = np.append(np.delete(restart_auto_detect_delta, [0]), control.delta)
                     restart_auto_detect_chg_grad = np.append(np.delete(restart_auto_detect_chg_grad, [0]), norm_chg_grad)
@@ -416,34 +418,34 @@
                     continue  # next iteration
                 else:
                     nruns_so_far += 1
                     break  # quit
 
             # Update delta
             if do_logging:
-                logging.debug("Ratio = %g" % ratio)
+                module_logger.debug("Ratio = %g" % ratio)
             if params("logging.save_diagnostic_info"):
                 diagnostic_info.update_ratio(ratio)
                 diagnostic_info.update_slow_iter(-1)  # n/a, unless otherwise update
             if ratio < params("tr_radius.eta1"):  # ratio < 0.1
                 control.delta = min(params("tr_radius.gamma_dec") * control.delta, dnorm)
                 if params("logging.save_diagnostic_info"):
-                    # logging.info("Last eval was for unsuccessful step (ratio = %g)" % ratio)
+                    # module_logger.info("Last eval was for unsuccessful step (ratio = %g)" % ratio)
                     diagnostic_info.update_iter_type(ITER_ACCEPTABLE_NO_GEOM if ratio > 0.0
                                                      else ITER_UNSUCCESSFUL_NO_GEOM)  # we flag geom update below
             elif ratio <= params("tr_radius.eta2"):  # 0.1 <= ratio <= 0.7
                 control.delta = max(params("tr_radius.gamma_dec") * control.delta, dnorm)
                 if params("logging.save_diagnostic_info"):
-                    # logging.info("Last eval was for acceptable step (ratio = %g)" % ratio)
+                    # module_logger.info("Last eval was for acceptable step (ratio = %g)" % ratio)
                     diagnostic_info.update_iter_type(ITER_SUCCESSFUL)
             else:  # (ratio > eta2 = 0.7)
                 control.delta = min(max(params("tr_radius.gamma_inc") * control.delta,
                                         params("tr_radius.gamma_inc_overline") * dnorm), 1.0e10)
                 if params("logging.save_diagnostic_info"):
-                    # logging.info("Last eval was for successful step (ratio = %g)" % ratio)
+                    # module_logger.info("Last eval was for successful step (ratio = %g)" % ratio)
                     diagnostic_info.update_iter_type(ITER_VERY_SUCCESSFUL)
             if control.delta <= 1.5 * control.rho:  # cap trust region radius at rho
                 control.delta = control.rho
 
             # Steps for successful steps
             if ratio > 0.0:
                 # Re-select knew, allowing knew=kopt this time
@@ -468,27 +470,27 @@
                         continue  # next iteration
                     else:
                         nruns_so_far += 1
                         break  # quit
 
             # Update point
             if do_logging:
-                logging.debug("Updating with knew = %i" % knew)
+                module_logger.debug("Updating with knew = %i" % knew)
             control.model.change_point(knew, xnew, f_list[0])  # expect step, not absolute x
             for i in range(1, num_samples_run):
                 control.model.add_new_sample(knew, f_extra=f_list[i])
 
             # Termination check: slow iterations [needs to be after updated with new point, as use model.fopt()
             if ratio > 0.0:
                 this_iter_slow, should_terminate = control.terminate_from_slow_iterations(current_iter, params)
                 if params("logging.save_diagnostic_info"):
                     diagnostic_info.update_slow_iter(1 if this_iter_slow else 0)
                 if should_terminate:
                     if do_logging:
-                        logging.info("Slow iteration  - terminating/restarting")
+                        module_logger.info("Slow iteration  - terminating/restarting")
                     if params("restarts.use_restarts") and params("restarts.use_soft_restarts"):
                         number_of_samples = max(nsamples(control.delta, control.rho, current_iter, nruns_so_far), 1)
                         exit_info = control.soft_restart(number_of_samples, nruns_so_far, params,
                                                          x_in_abs_coords_to_save=None, f_to_save=None,
                                                          nsamples_to_save=None)
                         if exit_info is not None:
                             nruns_so_far += 1
@@ -535,28 +537,28 @@
                     if control.model.npt() > control.n() + 1:
                         slope2, intercept2, r_value2, p_value2, std_err2 = STAT.linregress(np.arange(len(restart_auto_detect_chg_hess)),
                                                                                   np.log(np.maximum(restart_auto_detect_chg_hess, 1e-15)))
                     else:
                         slope2, intercept2, r_value2, p_value2, std_err2 = slope, intercept, r_value, p_value, std_err
 
                     if do_logging:
-                        logging.debug("Iter %g: (slope, intercept, r_value) = (%g, %g, %g)" % (current_iter, slope, intercept, r_value))
+                        module_logger.debug("Iter %g: (slope, intercept, r_value) = (%g, %g, %g)" % (current_iter, slope, intercept, r_value))
                     if min(slope, slope2) > params("restarts.auto_detect.min_chg_model_slope") \
                             and min(r_value, r_value2) > params("restarts.auto_detect.min_correl"):
                         # increasing trend, with at least some positive correlation
                         do_restart = True
                     else:
                         do_restart = False
 
                 if do_restart and params("restarts.use_soft_restarts"):
                     if do_logging:
-                        logging.info("Auto detection: need to do a restart")
-                        logging.debug("delta history = %s" % str(restart_auto_detect_delta))
-                        logging.debug("chg_grad history = %s" % str(restart_auto_detect_chg_grad))
-                        logging.debug("chg_hess history = %s" % str(restart_auto_detect_chg_hess))
+                        module_logger.info("Auto detection: need to do a restart")
+                        module_logger.debug("delta history = %s" % str(restart_auto_detect_delta))
+                        module_logger.debug("chg_grad history = %s" % str(restart_auto_detect_chg_grad))
+                        module_logger.debug("chg_hess history = %s" % str(restart_auto_detect_chg_hess))
                     number_of_samples = max(nsamples(control.delta, control.rho, current_iter, nruns_so_far), 1)
                     exit_info = control.soft_restart(number_of_samples, nruns_so_far, params,
                                                      x_in_abs_coords_to_save=None, f_to_save=None,
                                                      nsamples_to_save=None)
                     if exit_info is not None:
                         nruns_so_far += 1
                         break  # quit
@@ -566,23 +568,23 @@
                     restart_auto_detect_full = False
                     restart_auto_detect_delta = -1.0 * np.ones((params("restarts.auto_detect.history"),))
                     restart_auto_detect_chg_grad = -1.0 * np.ones((params("restarts.auto_detect.history"),))
                     restart_auto_detect_chg_hess = -1.0 * np.ones((params("restarts.auto_detect.history"),))
                     continue  # next iteration
                 elif do_restart:
                     if do_logging:
-                        logging.info("Auto detection: need to do a restart")
+                        module_logger.info("Auto detection: need to do a restart")
                     exit_info = ExitInformation(EXIT_AUTO_DETECT_RESTART_WARNING, "Auto-detected restart")
                     nruns_so_far += 1
                     break  # quit
                     # If not doing restart, just continue as below (geom steps, etc.)
 
             # Otherwise (ratio < eta1 = 0.1), check & fix geometry
             if do_logging:
-                logging.debug("Checking and possibly improving geometry (unsuccessful step)")
+                module_logger.debug("Checking and possibly improving geometry (unsuccessful step)")
             distsq = max((2.0 * control.delta) ** 2, (10.0 * control.rho) ** 2)
             update_delta = False
             number_of_samples = max(nsamples(control.delta, control.rho, current_iter, nruns_so_far), 1)
             did_fix_geom, exit_info = control.check_and_fix_geometry(distsq, update_delta, number_of_samples, params)
             if dnorm > control.rho:
                 control.last_successful_iter = current_iter
 
@@ -620,20 +622,20 @@
             # Otherwise, ratio <= 0 (i.e. delta was reduced) and we didn't fix geometry - check if we need to reduce rho
             if max(control.delta, dnorm) > control.rho:
                 continue  # next iteration
             elif control.rho > rhoend:
                 # Reduce rho
                 control.reduce_rho(current_iter, params)
                 if do_logging:
-                    logging.info("New rho = %g after %i function evaluations" % (control.rho, control.nf))
+                    module_logger.info("New rho = %g after %i function evaluations" % (control.rho, control.nf))
                     if control.n() < params("logging.n_to_print_whole_x_vector"):
-                        logging.debug("Best so far: f = %.15g at x = " % (control.model.fopt())
+                        module_logger.debug("Best so far: f = %.15g at x = " % (control.model.fopt())
                                       + str(control.model.xopt(abs_coordinates=True)))
                     else:
-                        logging.debug("Best so far: f = %.15g at x = [...]" % (control.model.fopt()))
+                        module_logger.debug("Best so far: f = %.15g at x = [...]" % (control.model.fopt()))
                 continue  # next iteration
             else:
                 # Quit on rho=rhoend
                 if params("restarts.use_restarts") and params("restarts.use_soft_restarts"):
                     number_of_samples = max(nsamples(control.delta, control.rho, current_iter, nruns_so_far), 1)
                     exit_info = control.soft_restart(number_of_samples, nruns_so_far, params,
                                                      x_in_abs_coords_to_save=None, f_to_save=None, nsamples_to_save=None)
@@ -654,16 +656,16 @@
                     break  # quit
                     # (end trust region step)
     # (end main loop)
 
     # Quit & return the important information
     x, f, gradmin, hessmin, nsamples = control.model.get_final_results()
     if do_logging:
-        logging.debug("At return from solver, number of function evals = %i" % nf)
-        logging.debug("Smallest objective value = %.15g at x = " % f + str(x))
+        module_logger.debug("At return from solver, number of function evals = %i" % nf)
+        module_logger.debug("Smallest objective value = %.15g at x = " % f + str(x))
     return x, f, gradmin, hessmin, nsamples, control.nf, control.nx, nruns_so_far, exit_info, diagnostic_info
 
 
 def solve(objfun, x0, args=(), bounds=None, npt=None, rhobeg=None, rhoend=1e-8, maxfun=None, nsamples=None, user_params=None,
           objfun_has_noise=False, seek_global_minimum=False, scaling_within_bounds=False, do_logging=True, print_progress=False):
     n = len(x0)
     if type(x0) == list:
@@ -819,36 +821,36 @@
             exit_info.able_to_do_restart() and nruns - last_successful_run < params("restarts.max_unsuccessful_restarts")\
             and total_unsuccessful_restarts < params("restarts.max_unsuccessful_restarts_total"):
         _rhoend = params("restarts.rhoend_scale") * _rhoend
         
         if not reduction_last_run:
             _rhobeg = _rhobeg * params("restarts.rhobeg_scale_after_unsuccessful_restart")
         
-        logging.info("Restarting from finish point (f = %g) after %g function evals; using rhobeg = %g and rhoend = %g"
+        module_logger.info("Restarting from finish point (f = %g) after %g function evals; using rhobeg = %g and rhoend = %g"
                      % (fmin, nf, _rhobeg, _rhoend))
         if params("restarts.hard.use_old_fk"):
             xmin2, fmin2, gradmin2, hessmin2, nsamples2, nf, nx, nruns, exit_info, diagnostic_info = \
                 solve_main(objfun, xmin, args, xl, xu, npt, _rhobeg, _rhoend, maxfun, nruns, nf, nx, nsamples, params,
                             diagnostic_info, scaling_changes, f0_avg_old=fmin, f0_nsamples_old=nsamples_min, do_logging=do_logging, print_progress=print_progress)
         else:
             xmin2, fmin2, gradmin2, hessmin2, nsamples2, nf, nx, nruns, exit_info, diagnostic_info = \
                 solve_main(objfun, xmin, args, xl, xu, npt, _rhobeg, _rhoend, maxfun, nruns, nf, nx, nsamples, params,
                            diagnostic_info, scaling_changes, do_logging=do_logging, print_progress=print_progress)
 
         if fmin2 < fmin or np.isnan(fmin):
-            logging.info("Successful run with new f = %s compared to old f = %s" % (fmin2, fmin))
+            module_logger.info("Successful run with new f = %s compared to old f = %s" % (fmin2, fmin))
             last_successful_run = nruns
             (xmin, fmin, nsamples_min) = (xmin2, fmin2, nsamples2)
             if gradmin2 is not None:  # may be None if finished during setup phase, in which case just use old gradient
                 gradmin = gradmin2
             if hessmin2 is not None:  # may be None if finished during setup phase, in which case just use old Hessian
                 hessmin = hessmin2
             reduction_last_run = True
         else:
-            logging.info("Unsuccessful run with new f = %s compared to old f = %s" % (fmin2, fmin))
+            module_logger.info("Unsuccessful run with new f = %s compared to old f = %s" % (fmin2, fmin))
             reduction_last_run = False
             total_unsuccessful_restarts += 1
 
     if nruns - last_successful_run >= params("restarts.max_unsuccessful_restarts"):
         exit_info = ExitInformation(EXIT_SUCCESS, "Reached maximum number of consecutive unsuccessful restarts")
     elif total_unsuccessful_restarts >= params("restarts.max_unsuccessful_restarts_total"):
         exit_info = ExitInformation(EXIT_SUCCESS, "Reached maximum total number of unsuccessful restarts")
@@ -864,11 +866,11 @@
             hessmin = hessmin / np.outer(scaling_changes[1], scaling_changes[1])
     results = OptimResults(remove_scaling(xmin, scaling_changes), fmin, gradmin, hessmin, nf, nx, nruns, exit_flag, exit_msg)
     if params("logging.save_diagnostic_info"):
         df = diagnostic_info.to_dataframe(with_xk=params("logging.save_xk"))
         results.diagnostic_info = df
 
     if do_logging:
-        logging.info("Did a total of %g run(s)" % nruns)
+        module_logger.info("Did a total of %g run(s)" % nruns)
 
     return results
```

### Comparing `Py-BOBYQA-1.3/pybobyqa/trust_region.py` & `Py-BOBYQA-1.4/pybobyqa/trust_region.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 """
 
 # Ensure compatibility with Python 2
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from math import sqrt
 import numpy as np
+import warnings
+
 try:
     import trustregion
     USE_FORTRAN = True
 except ImportError:
     # Fall back to Python implementation
     USE_FORTRAN = False
 
@@ -67,15 +69,18 @@
                                  verbose_output=True)
 
     n = xopt.size
     assert xopt.shape == (n,), "xopt has wrong shape (should be vector)"
     assert g.shape == (n,), "g and xopt have incompatible sizes"
     assert len(H.shape) == 2, "H must be a matrix"
     assert H.shape == (n,n), "H and xopt have incompatible sizes"
-    assert np.allclose(H, H.T), "H must be symmetric"
+    if not np.allclose(H, H.T):
+        # Enforce symmetry
+        H = 0.5 * (H + H.T)
+        warnings.warn("Trust-region solver: fixing non-symmetric Hessian", RuntimeWarning)
     assert sl.shape == (n,), "sl and xopt have incompatible sizes"
     assert su.shape == (n,), "su and xopt have incompatible sizes"
     assert delta > 0.0, "delta must be strictly positive"
     # Assume g and H have full quadratic model for objective
     # i.e. skip straight to label 8 in DFBOLS version
 
     # The sign of G(I) gives the sign of the change to the I-th variable
```

### Comparing `Py-BOBYQA-1.3/pybobyqa/util.py` & `Py-BOBYQA-1.4/pybobyqa/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 import numpy as np
 import sys
 
 
 __all__ = ['sumsq', 'eval_objective', 'model_value', 'random_orthog_directions_within_bounds',
            'random_directions_within_bounds', 'apply_scaling', 'remove_scaling']
 
+module_logger = logging.getLogger(__name__) 
+
 
 def sumsq(x):
     # There are several ways to calculate sum of squares of a vector:
     #   np.dot(x,x)
     #   np.sum(x**2)
     #   np.sum(np.square(x))
     #   etc.
@@ -52,17 +54,17 @@
         except OverflowError:
             f = sys.float_info.max
     else:
         f = objfun(x, *args)
 
     if verbose:
         if len(x) < full_x_thresh:
-            logging.info("Function eval %i at point %i has f = %.15g at x = " % (eval_num, pt_num, f) + str(x))
+            module_logger.info("Function eval %i at point %i has f = %.15g at x = " % (eval_num, pt_num, f) + str(x))
         else:
-            logging.info("Function eval %i at point %i has f = %.15g at x = [...]" % (eval_num, pt_num, f))
+            module_logger.info("Function eval %i at point %i has f = %.15g at x = [...]" % (eval_num, pt_num, f))
 
     return f
 
 
 def model_value(g, H, s):
     # Calculate model value (s^T * g + 0.5* s^T * H * s) = s^T * (gopt + 0.5 * H*s)
     assert g.shape == s.shape, "g and s have incompatible sizes"
```

### Comparing `Py-BOBYQA-1.3/pybobyqa/version.py` & `Py-BOBYQA-1.4/pybobyqa/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 The development of this software was sponsored by NAG Ltd. (http://www.nag.co.uk)
 and the EPSRC Centre For Doctoral Training in Industrially Focused Mathematical
 Modelling (EP/L015803/1) at the University of Oxford. Please contact NAG for
 alternative licensing.
 
 """
 
-__version__ = '1.3'
+__version__ = '1.4'
```

### Comparing `Py-BOBYQA-1.3/pybobyqa/__init__.py` & `Py-BOBYQA-1.4/pybobyqa/__init__.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.3/Py_BOBYQA.egg-info/PKG-INFO` & `Py-BOBYQA-1.4/Py_BOBYQA.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: Py-BOBYQA
-Version: 1.3
+Version: 1.4
 Summary: A flexible derivative-free solver for (bound constrained) general objective minimization
 Home-page: https://github.com/numericalalgorithmsgroup/pybobyqa/
 Author: Lindon Roberts
-Author-email: lindon.roberts@maths.ox.ac.uk
+Author-email: lindon.roberts@sydney.edu.au
 License: GNU GPL
-Download-URL: https://github.com/numericalalgorithmsgroup/pybobyqa/archive/v1.3.tar.gz
+Download-URL: https://github.com/numericalalgorithmsgroup/pybobyqa/archive/v1.4.tar.gz
 Description: ====================================================================
         Py-BOBYQA: Derivative-Free Solver for Bound-Constrained Minimization
         ====================================================================
         
-        .. image::  https://travis-ci.org/numericalalgorithmsgroup/pybobyqa.svg?branch=master
-           :target: https://travis-ci.org/numericalalgorithmsgroup/pybobyqa
+        .. image::  https://github.com/numericalalgorithmsgroup/pybobyqa/actions/workflows/python_testing.yml/badge.svg
+           :target: https://github.com/numericalalgorithmsgroup/pybobyqa/actions
            :alt: Build Status
         
         .. image::  https://img.shields.io/badge/License-GPL%20v3-blue.svg
            :target: https://www.gnu.org/licenses/gpl-3.0
            :alt: GNU GPL v3 License
         
         .. image:: https://img.shields.io/pypi/v/Py-BOBYQA.svg
            :target: https://pypi.python.org/pypi/Py-BOBYQA
            :alt: Latest PyPI version
         
         .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2630437.svg
            :target: https://doi.org/10.5281/zenodo.2630437
            :alt: DOI:10.5281/zenodo.2630437
         
+        .. image:: https://static.pepy.tech/personalized-badge/py-bobyqa?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads
+         :target: https://pepy.tech/project/py-bobyqa
+           :alt: Total downloads
+        
         Py-BOBYQA is a flexible package for solving bound-constrained general objective minimization, without requiring derivatives of the objective. At its core, it is a Python implementation of the BOBYQA algorithm by Powell, but Py-BOBYQA has extra features improving its performance on some problems (see the papers below for details). Py-BOBYQA is particularly useful when evaluations of the objective function are expensive and/or noisy.
         
         More details about Py-BOBYQA and its enhancements over BOBYQA can be found in our papers:
         
         1. Coralia Cartis, Jan Fiala, Benjamin Marteau and Lindon Roberts, `Improving the Flexibility and Robustness of Model-Based Derivative-Free Optimization Solvers <https://doi.org/10.1145/3338517>`_, *ACM Transactions on Mathematical Software*, 45:3 (2019), pp. 32:1-32:41 [`arXiv preprint: 1804.00154 <https://arxiv.org/abs/1804.00154>`_] 
         2. Coralia Cartis, Lindon Roberts and Oliver Sheridan-Methven, `Escaping local minima with derivative-free methods: a numerical investigation <https://doi.org/10.1080/02331934.2021.1883015>`_, *Optimization* (2021). [`arXiv preprint: 1812.11343 <https://arxiv.org/abs/1812.11343>`_]
```

### Comparing `Py-BOBYQA-1.3/README.rst` & `Py-BOBYQA-1.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 ====================================================================
 Py-BOBYQA: Derivative-Free Solver for Bound-Constrained Minimization
 ====================================================================
 
-.. image::  https://travis-ci.org/numericalalgorithmsgroup/pybobyqa.svg?branch=master
-   :target: https://travis-ci.org/numericalalgorithmsgroup/pybobyqa
+.. image::  https://github.com/numericalalgorithmsgroup/pybobyqa/actions/workflows/python_testing.yml/badge.svg
+   :target: https://github.com/numericalalgorithmsgroup/pybobyqa/actions
    :alt: Build Status
 
 .. image::  https://img.shields.io/badge/License-GPL%20v3-blue.svg
    :target: https://www.gnu.org/licenses/gpl-3.0
    :alt: GNU GPL v3 License
 
 .. image:: https://img.shields.io/pypi/v/Py-BOBYQA.svg
    :target: https://pypi.python.org/pypi/Py-BOBYQA
    :alt: Latest PyPI version
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2630437.svg
    :target: https://doi.org/10.5281/zenodo.2630437
    :alt: DOI:10.5281/zenodo.2630437
 
+.. image:: https://static.pepy.tech/personalized-badge/py-bobyqa?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads
+ :target: https://pepy.tech/project/py-bobyqa
+   :alt: Total downloads
+
 Py-BOBYQA is a flexible package for solving bound-constrained general objective minimization, without requiring derivatives of the objective. At its core, it is a Python implementation of the BOBYQA algorithm by Powell, but Py-BOBYQA has extra features improving its performance on some problems (see the papers below for details). Py-BOBYQA is particularly useful when evaluations of the objective function are expensive and/or noisy.
 
 More details about Py-BOBYQA and its enhancements over BOBYQA can be found in our papers:
 
 1. Coralia Cartis, Jan Fiala, Benjamin Marteau and Lindon Roberts, `Improving the Flexibility and Robustness of Model-Based Derivative-Free Optimization Solvers <https://doi.org/10.1145/3338517>`_, *ACM Transactions on Mathematical Software*, 45:3 (2019), pp. 32:1-32:41 [`arXiv preprint: 1804.00154 <https://arxiv.org/abs/1804.00154>`_] 
 2. Coralia Cartis, Lindon Roberts and Oliver Sheridan-Methven, `Escaping local minima with derivative-free methods: a numerical investigation <https://doi.org/10.1080/02331934.2021.1883015>`_, *Optimization* (2021). [`arXiv preprint: 1812.11343 <https://arxiv.org/abs/1812.11343>`_]
```

### Comparing `Py-BOBYQA-1.3/setup.py` & `Py-BOBYQA-1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 
 setup(
     name='Py-BOBYQA',
     version=__version__,
     description='A flexible derivative-free solver for (bound constrained) general objective minimization',
     long_description=open('README.rst').read(),
     author='Lindon Roberts',
-    author_email='lindon.roberts@maths.ox.ac.uk',
+    author_email='lindon.roberts@sydney.edu.au',
     url="https://github.com/numericalalgorithmsgroup/pybobyqa/",
-    download_url="https://github.com/numericalalgorithmsgroup/pybobyqa/archive/v1.3.tar.gz",
+    download_url="https://github.com/numericalalgorithmsgroup/pybobyqa/archive/v1.4.tar.gz",
     packages=['pybobyqa'],
     license='GNU GPL',
     keywords = "mathematics derivative free optimization",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Framework :: IPython',
```

