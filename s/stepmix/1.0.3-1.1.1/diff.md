# Comparing `tmp/stepmix-1.0.3.tar.gz` & `tmp/stepmix-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepmix-1.0.3.tar", last modified: Thu May 11 21:03:26 2023, max compression
+gzip compressed data, was "stepmix-1.1.1.tar", last modified: Tue May 16 18:14:27 2023, max compression
```

## Comparing `stepmix-1.0.3.tar` & `stepmix-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.0.3/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.0.3/.gitignore
--rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.0.3/.readthedocs.yaml
--rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.0.3/LICENSE
--rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.0.3/README-dev.md
--rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.0.3/README.md
--rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.0.3/docs/Makefile
--rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.0.3/docs/make.bat
--rw-r--r--   0        0        0      929 2023-01-11 22:01:14.079040 stepmix-1.0.3/docs/source/api.rst
--rw-r--r--   0        0        0     1016 2023-05-11 21:02:57.820805 stepmix-1.0.3/docs/source/conf.py
--rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.0.3/docs/source/index.rst
--rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.0.3/docs/source/installation.rst
--rw-r--r--   0        0        0     2814 2023-01-11 22:01:14.083040 stepmix-1.0.3/docs/source/tutorials.rst
--rw-r--r--   0        0        0     1872 2023-05-11 21:02:57.820805 stepmix-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      579 2023-04-25 21:29:34.007800 stepmix-1.0.3/scripts/README.md
--rwxr-xr-x   0        0        0     5603 2023-03-09 18:24:49.769774 stepmix-1.0.3/scripts/run_bakk_simulation.py
--rwxr-xr-x   0        0        0     4996 2023-03-09 22:19:26.676204 stepmix-1.0.3/scripts/run_bakk_simulation_complete.py
--rw-r--r--   0        0        0      174 2023-05-11 21:02:57.820805 stepmix-1.0.3/stepmix/__init__.py
--rw-r--r--   0        0        0     8489 2023-05-11 21:02:57.820805 stepmix-1.0.3/stepmix/bootstrap.py
--rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.0.3/stepmix/corrections.py
--rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.0.3/stepmix/datasets.py
--rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.0.3/stepmix/emission/__init__.py
--rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.0.3/stepmix/emission/build_emission.py
--rw-r--r--   0        0        0     6283 2023-03-09 22:19:26.676204 stepmix-1.0.3/stepmix/emission/categorical.py
--rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.0.3/stepmix/emission/covariate.py
--rw-r--r--   0        0        0     6031 2023-01-11 22:01:14.083040 stepmix-1.0.3/stepmix/emission/emission.py
--rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.0.3/stepmix/emission/gaussian.py
--rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.0.3/stepmix/emission/nested.py
--rw-r--r--   0        0        0    52639 2023-03-09 18:24:49.769774 stepmix-1.0.3/stepmix/stepmix.py
--rw-r--r--   0        0        0    18189 2023-04-30 21:21:22.007846 stepmix-1.0.3/stepmix/utils.py
--rw-r--r--   0        0        0     4074 2023-05-11 17:57:51.569120 stepmix-1.0.3/test/conftest.py
--rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.0.3/test/test_benchmarks.py
--rw-r--r--   0        0        0     5571 2023-05-11 21:02:57.820805 stepmix-1.0.3/test/test_bootstrap.py
--rw-r--r--   0        0        0     8818 2023-04-30 21:21:22.007846 stepmix-1.0.3/test/test_emission.py
--rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.0.3/test/test_fiml.py
--rw-r--r--   0        0        0     1781 2023-04-30 21:21:22.007846 stepmix-1.0.3/test/test_inputs.py
--rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.0.3/test/test_random_state.py
--rw-r--r--   0        0        0      795 2023-01-11 22:01:14.083040 stepmix-1.0.3/test/test_sklearn.py
--rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.0.3/test/test_steps.py
--rw-r--r--   0        0        0     6525 1970-01-01 00:00:00.000000 stepmix-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.1.1/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.1.1/.gitignore
+-rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.1.1/README-dev.md
+-rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.1.1/README.md
+-rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0     1051 2023-05-16 17:54:29.612732 stepmix-1.1.1/docs/source/api.rst
+-rw-r--r--   0        0        0     1016 2023-05-16 18:04:21.788860 stepmix-1.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.1.1/docs/source/installation.rst
+-rw-r--r--   0        0        0     3426 2023-05-16 17:54:29.612732 stepmix-1.1.1/docs/source/tutorials.rst
+-rw-r--r--   0        0        0     1884 2023-05-16 18:04:21.788860 stepmix-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      557 2023-05-16 17:54:29.612732 stepmix-1.1.1/scripts/README.md
+-rwxr-xr-x   0        0        0     5644 2023-05-16 17:54:29.612732 stepmix-1.1.1/scripts/run_bakk_simulation.py
+-rwxr-xr-x   0        0        0     5038 2023-05-16 17:54:29.612732 stepmix-1.1.1/scripts/run_bakk_simulation_complete.py
+-rw-r--r--   0        0        0      174 2023-05-16 18:04:21.788860 stepmix-1.1.1/stepmix/__init__.py
+-rw-r--r--   0        0        0    10272 2023-05-16 17:54:29.612732 stepmix-1.1.1/stepmix/bootstrap.py
+-rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.1.1/stepmix/corrections.py
+-rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.1.1/stepmix/datasets.py
+-rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.1.1/stepmix/emission/__init__.py
+-rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.1.1/stepmix/emission/build_emission.py
+-rw-r--r--   0        0        0     6283 2023-03-09 22:19:26.676204 stepmix-1.1.1/stepmix/emission/categorical.py
+-rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.1.1/stepmix/emission/covariate.py
+-rw-r--r--   0        0        0     6031 2023-01-11 22:01:14.083040 stepmix-1.1.1/stepmix/emission/emission.py
+-rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.1.1/stepmix/emission/gaussian.py
+-rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.1.1/stepmix/emission/nested.py
+-rw-r--r--   0        0        0    54258 2023-05-16 18:04:21.788860 stepmix-1.1.1/stepmix/stepmix.py
+-rw-r--r--   0        0        0    18715 2023-05-16 17:54:29.616732 stepmix-1.1.1/stepmix/utils.py
+-rw-r--r--   0        0        0     4074 2023-05-11 17:57:51.569120 stepmix-1.1.1/test/conftest.py
+-rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.1.1/test/test_benchmarks.py
+-rw-r--r--   0        0        0     5571 2023-05-11 21:02:57.820805 stepmix-1.1.1/test/test_bootstrap.py
+-rw-r--r--   0        0        0     8818 2023-04-30 21:21:22.007846 stepmix-1.1.1/test/test_emission.py
+-rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.1.1/test/test_fiml.py
+-rw-r--r--   0        0        0     1781 2023-04-30 21:21:22.007846 stepmix-1.1.1/test/test_inputs.py
+-rw-r--r--   0        0        0      337 2023-05-16 17:54:29.616732 stepmix-1.1.1/test/test_progress_bar.py
+-rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.1.1/test/test_random_state.py
+-rw-r--r--   0        0        0     2101 2023-05-16 17:54:29.616732 stepmix-1.1.1/test/test_sample_weight.py
+-rw-r--r--   0        0        0      795 2023-01-11 22:01:14.083040 stepmix-1.1.1/test/test_sklearn.py
+-rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.1.1/test/test_steps.py
+-rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 stepmix-1.1.1/PKG-INFO
```

### Comparing `stepmix-1.0.3/.github/workflows/pytest.yaml` & `stepmix-1.1.1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/LICENSE` & `stepmix-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/README-dev.md` & `stepmix-1.1.1/README-dev.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/README.md` & `stepmix-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/docs/Makefile` & `stepmix-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/docs/make.bat` & `stepmix-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/docs/source/api.rst` & `stepmix-1.1.1/docs/source/api.rst`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 .. autoclass:: stepmix.stepmix.StepMix
     :members:
     :undoc-members:
     :inherited-members:
     :show-inheritance:
 
+Bootstrap
+---------------
+.. automodule:: stepmix.bootstrap
+    :members:
+    :inherited-members:
+    :show-inheritance:
+
 Emission Models
 ---------------
 Categorical
 ~~~~~~~~~~~
 .. automodule:: stepmix.emission.categorical
     :members:
     :undoc-members:
```

### Comparing `stepmix-1.0.3/docs/source/conf.py` & `stepmix-1.1.1/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 sys.path.insert(0, os.path.abspath("../.."))
 
 project = "StepMix"
 copyright = "2022, Labo-Lacourse"
 author = "Sacha Morin, Robin Legault"
 
 release = "0.0"
-version = "1.0.3"
+version = "1.1.1"
 
 
 # -- General configuration
 
 extensions = [
     "sphinx.ext.napoleon",
     # 'numpydoc',
```

### Comparing `stepmix-1.0.3/docs/source/index.rst` & `stepmix-1.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/pyproject.toml` & `stepmix-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -27,25 +27,26 @@
 keywords = ["clustering", "mixtures", "lca", "em", "latent-class-analysis", "expectation–maximization"]
 dependencies = [
     "numpy",
     "pandas",
     "scikit-learn >= 1.0.0",
     "scipy",
     "matplotlib",
+    "tqdm",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "flit", "pytest", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 Homepage = "https://stepmix.readthedocs.io/en/latest/"
 
 [tool.bumpver]
-current_version = "1.0.3"
+current_version = "1.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `stepmix-1.0.3/scripts/README.md` & `stepmix-1.1.1/scripts/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 ==============================
 This directory provides the scripts to reproduce the simulations and tables from the Computational
 examples section of the StepMix paper. Results can be reproduced with the 
 following commands:
 
 ```bash
 # Outcome simulation
-python3 run_bakk_simulation.py -s 500 -l
+python3 run_bakk_simulation.py -s 500
 # Covariate simulation
-python3 run_bakk_simulation.py -s 500 -l -c
+python3 run_bakk_simulation.py -s 500 -c
 # Complete simulation
-python3 run_bakk_simulation_complete.py -s 500 -l
+python3 run_bakk_simulation_complete.py -s 500
 ```
-All three commands should output the latex tables from the paper, up to formatting. You can ignore the UserWarnings.
+All three commands should output the simulation tables from the paper. You can ignore the UserWarnings.
```

### Comparing `stepmix-1.0.3/scripts/run_bakk_simulation.py` & `stepmix-1.1.1/scripts/run_bakk_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         help="Number of simulations to run. Results are averaged.",
         type=int,
         default=10,
     )
     parser.add_argument(
         "--latex",
         "-l",
-        help="Also print a latex version of the results.",
+        help="Also print a latex version of the results. Requires the optional dependency Jinja2.",
         action="store_true",
     )
     parser.add_argument(
         "--covariate",
         "-c",
         help="Run the covariate simulation. Otherwise runs the response simulation by default.",
         action="store_true",
```

### Comparing `stepmix-1.0.3/scripts/run_bakk_simulation_complete.py` & `stepmix-1.1.1/scripts/run_bakk_simulation_complete.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,13 +150,13 @@
         help="Number of simulations to run. Results are averaged.",
         type=int,
         default=10,
     )
     parser.add_argument(
         "--latex",
         "-l",
-        help="Also print a latex version of the results.",
+        help="Also print a latex version of the results.  Requires the optional dependency Jinja2.",
         action="store_true",
     )
 
     args = parser.parse_args()
     main(n_simulations=args.n_simulations, latex=args.latex)
```

### Comparing `stepmix-1.0.3/stepmix/bootstrap.py` & `stepmix-1.1.1/stepmix/bootstrap.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import copy
 import itertools
 import math
 
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
+import tqdm
 
 from sklearn.base import clone
 from sklearn.utils.validation import check_random_state
 
 
 def mse(x, y):
     return np.square(np.subtract(x, y)).mean()
@@ -66,75 +67,123 @@
                 base[key_i][key_j] = np.stack([p[key_i][key_j] for p in params])
 
     base["weights"] = np.stack([p["weights"] for p in params])
 
     return base
 
 
-def bootstrap(estimator, X, Y=None, n_repetitions=1000):
+def bootstrap(
+    estimator, X, Y=None, sample_weight=None, n_repetitions=1000, progress_bar=True
+):
     """Non-parametric boostrap of StepMix estimator.
 
     Fit the estimator on X,Y then fit n_repetitions on resampled datasets.
 
     Repetition parameters are aligned with the class order of the main estimator.
 
     Parameters
     ----------
     estimator : StepMix instance
         Estimator to use for bootstrapping.
     X : array-like of shape (n_samples, n_columns)
         Measurement data.
     Y : array-like of shape (n_samples, n_columns_structural), default=None
         Structural data.
+    sample_weight : array-like of shape(n_samples,), default=None
+        Array of weights that are assigned to individual samples.
+        If not provided, then each sample is given unit weight.
     n_repetitions: int
         Number of repetitions to fit.
+    progress_bar : bool, default=True
+        Display a tqdm progress bar for repetitions.
     Returns
     ----------
     estimator: StepMix
         Fitted instance of the estimator.
-    parameters: ndarray
+    parameters: Dict
         StepMix parameter dictionary. Follows the same convention as the parameters of the StepMix
         object. An additional axis of size (n_repetitions,) is added at position 0 of each parameter array.
+        Additional "LL" and "avg_LL" keys contain the likelihood and average likelihood of different repetitions.
     """
     n_samples = X.shape[0]
 
     # Use the estimator built-in method to check the input
     # This will ensure that X and Y are numpy arrays for the rest of the bootstrap procedure
     estimator._check_initial_parameters(X)
     X, Y = estimator._check_x_y(X, Y, reset=True)
 
     # First fit the base estimator and get class probabilities
-    estimator.fit(X, Y)
+    estimator.fit(X, Y, sample_weight=sample_weight)
     ref_class_probabilities = estimator.predict_proba(X, Y)
 
-    # Not fit n_repetitions estimator with resampling and save parameters
+    # Now fit n_repetitions estimator with resampling and save parameters
     rng = check_random_state(estimator.random_state)
     parameters = list()
+    avg_ll_buffer = list()
+    ll_buffer = list()
 
-    for _ in range(n_repetitions):
+    if progress_bar:
+        print("\nBootstrapping estimator...")
+
+    tqdm_rep = tqdm.trange(
+        n_repetitions, disable=not progress_bar, desc="Bootstrap Repetitions    "
+    )
+    for _ in tqdm_rep:
         # Resample data
         rep_samples = rng.choice(n_samples, size=(n_samples,), replace=True)
         X_rep = X[rep_samples]
         Y_rep = Y[rep_samples] if Y is not None else None
+        sample_weight_rep = (
+            sample_weight[rep_samples] if sample_weight is not None else None
+        )
 
         # Fit estimator on resample data
         estimator_rep = clone(estimator)
-        estimator_rep.fit(X_rep, Y_rep)
+
+        # Disable printing for repeated estimators and fit
+        estimator_rep.verbose = 0
+        estimator_rep.progress_bar = 0
+        estimator_rep.fit(X_rep, Y_rep, sample_weight=sample_weight_rep)
 
         # Class ordering may be different. Reorder based on best permutation of class probabilites
         rep_class_probabilities = estimator_rep.predict_proba(
             X, Y
         )  # Inference on original samples
         perm = find_best_permutation(ref_class_probabilities, rep_class_probabilities)
         estimator_rep.permute_classes(perm)
 
         # Save parameters
         parameters.append(estimator_rep.get_parameters())
 
-    return estimator, stack_stepmix_parameters(parameters)
+        # Save likelihood
+        avg_ll = estimator_rep.score(X_rep, Y_rep, sample_weight=sample_weight_rep)
+        ll = (
+            avg_ll * np.sum(sample_weight)
+            if sample_weight is not None
+            else avg_ll * n_samples
+        )
+        avg_ll_buffer.append(avg_ll)
+        ll_buffer.append(ll)
+
+        # Ask tqdm to display current max likelihood
+        tqdm_rep.set_postfix(
+            median_LL=np.median(ll_buffer),
+            # min_avg_LL=np.min(avg_ll_buffer),
+            # max_avg_LL=np.max(avg_ll_buffer),
+            min_LL=np.min(ll_buffer),
+            max_LL=np.max(ll_buffer),
+        )
+
+    return_dict = stack_stepmix_parameters(parameters)
+
+    # Add likelihoods statistics
+    return_dict["LL"] = np.array(ll_buffer)
+    return_dict["avg_LL"] = np.array(avg_ll_buffer)
+
+    return estimator, return_dict
 
 
 def plot_CI(bottom, estimate, top, ax):
     """Adapted from https://stackoverflow.com/questions/59747313/how-can-i-plot-a-confidence-interval-in-python."""
     horizontal_line_width = 0.25
     color = "#2187bb"
```

### Comparing `stepmix-1.0.3/stepmix/corrections.py` & `stepmix-1.1.1/stepmix/corrections.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/stepmix/datasets.py` & `stepmix-1.1.1/stepmix/datasets.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/stepmix/emission/build_emission.py` & `stepmix-1.1.1/stepmix/emission/build_emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/stepmix/emission/categorical.py` & `stepmix-1.1.1/stepmix/emission/categorical.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/stepmix/emission/covariate.py` & `stepmix-1.1.1/stepmix/emission/covariate.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/stepmix/emission/emission.py` & `stepmix-1.1.1/stepmix/emission/emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/stepmix/emission/gaussian.py` & `stepmix-1.1.1/stepmix/emission/gaussian.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/stepmix/emission/nested.py` & `stepmix-1.1.1/stepmix/emission/nested.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/stepmix/stepmix.py` & `stepmix-1.1.1/stepmix/stepmix.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from sklearn.exceptions import ConvergenceWarning
 from sklearn.utils.validation import (
     check_random_state,
     check_is_fitted,
     _check_sample_weight,
 )
 from sklearn.cluster import KMeans
+import tqdm
 
 from . import utils
 from .corrections import compute_bch_matrix, compute_log_emission_pm
 from .emission.build_emission import EMISSION_DICT, build_emission
 
 
 class StepMix(BaseEstimator):
@@ -130,16 +131,22 @@
             - 'random' : responsibilities are initialized randomly.
 
     random_state : int, RandomState instance or None, default=None
         Controls the random seed given to the method chosen to initialize the
         parameters. Pass an int for reproducible output across multiple function calls.
     verbose : int, default=0
         Enable verbose output. If 1, will print detailed report of the model and the performance metrics after fitting.
-    verbose_interval : int, default=10
-        Number of iteration done before the next print. TODO: Not currently implemented.
+    progress_bar : int, default=1
+        Display a tqdm progress bar during fitting.
+
+            - 0 : No progress bar.
+            - 1 : Progress bar for initializations.
+            - 2 : Progress bars for initializations and iterations. This requires a nested tqdm bar and may not work\
+            properly in some terminals.
+
     measurement_params: {dict, None}, default=None
         Additional params passed to the measurement model class.  Particularly useful to specify optimization parameters
         for :class:`stepmix.emission.covariate.Covariate`. Ignored if the measurement descriptor is a nested object
         (see :class:`stepmix.emission.nested.Nested`).
     structural_params: {dict, None}, default=None
         Additional params passed to the structural model class.  Particularly useful to specify optimization parameters
         for :class:`stepmix.emission.covariate.Covariate`. Ignored if the structural descriptor is a nested object
@@ -217,28 +224,28 @@
         abs_tol=1e-10,
         rel_tol=0.00,
         max_iter=1000,
         n_init=1,
         init_params="random",
         random_state=None,
         verbose=0,
-        verbose_interval=10,
+        progress_bar=1,
         measurement_params=None,
         structural_params=None,
     ):
         # Attributes of the base StepMix class
         self.n_components = n_components
         self.abs_tol = abs_tol
         self.rel_tol = rel_tol
         self.max_iter = max_iter
         self.n_init = n_init
         self.init_params = init_params
         self.random_state = random_state
         self.verbose = verbose
-        self.verbose_interval = verbose_interval
+        self.progress_bar = progress_bar
         self.n_steps = n_steps
 
         # Additional attributes for 3-step estimation
         self.assignment = assignment
         self.correction = correction
 
         # Additional attributes to specify the measurement and structural models
@@ -264,25 +271,24 @@
         """
         utils.check_type(
             int,
             n_components=self.n_components,
             max_iter=self.max_iter,
             n_init=self.n_init,
             verbose=self.verbose,
-            verbose_interval=self.verbose_interval,
         )
         utils.check_positive(
             n_components=self.n_components,
             max_iter=self.max_iter,
             n_init=self.n_init,
-            verbose_interval=self.verbose_interval,
         )
         utils.check_nonneg(abs_tol=self.abs_tol, verbose=self.verbose)
         utils.check_nonneg(rel_tol=self.rel_tol, verbose=self.verbose)
         utils.check_in([1, 2, 3], n_steps=self.n_steps)
+        utils.check_in([0, 1, 2], progress_bar=self.progress_bar)
         utils.check_in(["kmeans", "random"], init_params=self.init_params)
         utils.check_in(["modal", "soft"], init_params=self.assignment)
         utils.check_in([None, "BCH", "ML"], init_params=self.correction)
         utils.check_descriptor(self.measurement, keys=EMISSION_DICT.keys())
         utils.check_descriptor(self.structural, keys=EMISSION_DICT.keys())
         utils.check_type(
             (dict, type(None)),
@@ -662,19 +668,19 @@
             log_emission_pm = compute_log_emission_pm(soft_resp, self.assignment)
 
             # 3) Fit the structural model by keeping the parameters of the measurement model fixed
             self.em(X, Y, freeze_measurement=True, log_emission_pm=log_emission_pm)
 
         # Print report if required
         if self.verbose == 1:
-            self.report(X, Y)
+            self.report(X, Y, sample_weight=sample_weight)
 
         return self
 
-    def report(self, X, Y=None):
+    def report(self, X, Y=None, sample_weight=None):
         """Print detailed report of the model and performance metrics.
 
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_columns)
             List of n_features-dimensional data points, where each column corresponds
@@ -684,16 +690,19 @@
             data point of the measurement model.
         Y : array-like of shape (n_samples, n_columns_structural), default=None
             List of n_features-dimensional data points, where each column corresponds
             to a feature for univariate variables (n_features=n_columns_structural)
             and each group of L columns corresponds to a feature for one-hot encoded
             variables with L possible outcomes (n_features=n_columns_structural/L).
             Each row corresponds to a  single data point of the structural model.
+        sample_weight : array-like of shape(n_samples,), default=None
+            Array of weights that are assigned to individual samples.
+            If not provided, then each sample is given unit weight.
         """
-        utils.print_report(self, X, Y)
+        utils.print_report(self, X, Y, sample_weight)
 
     def em(
         self,
         X,
         Y=None,
         sample_weight=None,
         freeze_measurement=False,
@@ -750,29 +759,42 @@
 
         # Set up useful values for optimization
         random_state = check_random_state(self.random_state)
         max_lower_bound = -np.inf
         self.converged_ = False
 
         # Run multiple restarts
-        for init in range(self.n_init):
-            # self._print_verbose_msg_init_beg(init)
-
+        if self.progress_bar:
+            print("Fitting StepMix...")
+        if self.progress_bar == 2:
+            print(
+                "The Iteration bar may update too quickly to be visualized depending on dataset size and StepMix settings.\n"
+            )
+        tqdm_init = tqdm.trange(
+            self.n_init, disable=not self.progress_bar, desc="Initializations (n_init) "
+        )
+        for init in tqdm_init:
             if not freeze_measurement:
                 self._initialize_parameters(X, random_state)  # Measurement model
 
             if Y is not None:
                 self._initialize_parameters_structural(
                     Y, random_state
                 )  # Structural Model
 
             lower_bound = -np.inf
 
             # EM iterations
-            for n_iter in range(1, self.max_iter + 1):
+            tqdm_iter = tqdm.tqdm(
+                range(1, self.max_iter + 1),
+                disable=self.progress_bar < 2,
+                desc="Iterations (max_iter)    ",
+                leave=False,
+            )
+            for n_iter in tqdm_iter:
                 prev_lower_bound = lower_bound
 
                 # E-step
                 log_prob_norm, log_resp = self._e_step(
                     X, Y=Y, sample_weight=sample_weight, log_emission_pm=log_emission_pm
                 )
 
@@ -795,23 +817,39 @@
 
                 # if both an absolute and a relative tolerance threshold are given, the EM algorithm stops
                 # as soon as one of them is respected
                 if abs(change) < self.abs_tol or abs(rel_change) < self.rel_tol:
                     self.converged_ = True
                     break
 
+                # Ask tqdm to display current max lower bound
+                ll = (
+                    lower_bound * np.sum(sample_weight)
+                    if sample_weight is not None
+                    else lower_bound * n_samples
+                )
+                tqdm_iter.set_postfix(avg_LL=lower_bound, LL=ll)
+
             if (
                 lower_bound > max_lower_bound
                 or max_lower_bound == -np.inf
                 or np.isnan(max_lower_bound)
             ):
                 max_lower_bound = lower_bound
                 best_params = self.get_parameters()
                 best_n_iter = n_iter
 
+            # Ask tqdm to display current max lower bound
+            max_ll = (
+                max_lower_bound * np.sum(sample_weight)
+                if sample_weight is not None
+                else max_lower_bound * n_samples
+            )
+            tqdm_init.set_postfix(max_avg_LL=max_lower_bound, max_LL=max_ll)
+
         if not self.converged_:
             warnings.warn(
                 "Initializations did not converge. "
                 "Try different init parameters, "
                 "or increase max_iter, abs_tol, rel_tol "
                 "or check for degenerate data.",
                 ConvergenceWarning,
```

### Comparing `stepmix-1.0.3/stepmix/utils.py` & `stepmix-1.1.1/stepmix/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,15 +276,15 @@
 
     if clip:
         modal_resp = np.clip(modal_resp, 1e-15, 1 - 1e-15)
 
     return modal_resp
 
 
-def print_report(model, X, Y=None):
+def print_report(model, X, Y=None, sample_weight=None):
     """Print detailed output for the model.
 
     Parameters
     ----------
     model: stepmix.StepMix
         Fitted StepMix instance.
     X : array-like of shape (n_samples, n_columns)
@@ -295,20 +295,30 @@
             data point of the measurement model.
     Y : array-like of shape (n_samples, n_columns_structural), default=None
         List of n_features-dimensional data points, where each column corresponds
         to a feature for univariate variables (n_features=n_columns_structural)
         and each group of L columns corresponds to a feature for one-hot encoded
         variables with L possible outcomes (n_features=n_columns_structural/L).
         Each row corresponds to a  single data point of the structural model.
+    sample_weight : array-like of shape(n_samples,), default=None
+        Array of weights that are assigned to individual samples.
+        If not provided, then each sample is given unit weight.
     """
     check_is_fitted(model)
     n_classes = model.n_components
     n_samples = X.shape[0]
     n_parameters = model.n_parameters
-    ll = model.score(X, Y)
+    avg_ll = model.score(X, Y, sample_weight=sample_weight)
+    ll = (
+        avg_ll * np.sum(sample_weight)
+        if sample_weight is not None
+        else avg_ll * n_samples
+    )
+    minus2ll = -2 * ll
+
     bic = model.bic(X, Y)
     aic = model.aic(X, Y)
 
     print("=" * 80)
     print("MODEL REPORT")
     print("=" * 80)
     print("    " + "=" * 76)
@@ -334,15 +344,17 @@
     print(f"    Estimation method             : {model.n_steps}-step")
     if model.n_steps == 3:
         print(f"    Correction method             : {model.correction}")
         print(f"    Assignment method             : {model.assignment}")
     print(f"    Number of observations        : {n_samples}")
     print(f"    Number of latent classes      : {n_classes}")
     print(f"    Number of estimated parameters: {n_parameters}")
-    print(f"    Average log-likelihood        : {ll:.4f}")
+    print(f"    Log-likelihood (LL)           : {ll:.4f}")
+    print(f"    -2LL                          : {minus2ll:.4f}")
+    print(f"    Average LL                    : {avg_ll:.4f}")
     print(f"    AIC                           : {aic:.2f}")
     print(f"    BIC                           : {bic:.2f}")
 
 
 def print_parameters(
     params,
     model_name,
```

### Comparing `stepmix-1.0.3/test/conftest.py` & `stepmix-1.1.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/test/test_benchmarks.py` & `stepmix-1.1.1/test/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/test/test_bootstrap.py` & `stepmix-1.1.1/test/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/test/test_emission.py` & `stepmix-1.1.1/test/test_emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/test/test_fiml.py` & `stepmix-1.1.1/test/test_fiml.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/test/test_inputs.py` & `stepmix-1.1.1/test/test_inputs.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/test/test_random_state.py` & `stepmix-1.1.1/test/test_random_state.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/test/test_sklearn.py` & `stepmix-1.1.1/test/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/test/test_steps.py` & `stepmix-1.1.1/test/test_steps.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.0.3/PKG-INFO` & `stepmix-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: stepmix
-Version: 1.0.3
+Version: 1.1.1
 Summary: A Python package for stepwise estimation of latent class models with measurement and structural components. The package can also be used to fit mixture models with various observed random variables.
 Keywords: clustering,mixtures,lca,em,latent-class-analysis,expectation–maximization
 Author-email: Sacha Morin <sacha.morin@mila.quebec>, Robin Legault <robin.legault@umontreal.ca>, Charles-Édouard Giguère <ce.giguere@gmail.com>, Éric Lacourse <eric.lacourse@umontreal.ca>, Roxane de la Sablonnière <roxane.de.la.sablonniere@umontreal.ca>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn >= 1.0.0
 Requires-Dist: scipy
 Requires-Dist: matplotlib
+Requires-Dist: tqdm
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: sphinx ; extra == "dev"
 Requires-Dist: sphinx-rtd-theme ; extra == "dev"
 Project-URL: Homepage, https://stepmix.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: stepmix Version: 1.0.3 Summary: A Python package
+Metadata-Version: 2.1 Name: stepmix Version: 1.1.1 Summary: A Python package
 for stepwise estimation of latent class models with measurement and structural
 components. The package can also be used to fit mixture models with various
 observed random variables. Keywords: clustering,mixtures,lca,em,latent-class-
 analysis,expectationâmaximization Author-email: Sacha Morin
 morin@mila.quebec>, Robin Legault
 legault@umontreal.ca>, Charles-Ãdouard GiguÃ¨re
 giguere@gmail.com>, Ãric Lacourse
 lacourse@umontreal.ca>, Roxane de la SablonniÃ¨re
 de.la.sablonniere@umontreal.ca> Requires-Python: >=3.7 Description-Content-
 Type: text/markdown Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: scikit-
 learn >= 1.0.0 Requires-Dist: scipy Requires-Dist: matplotlib Requires-Dist:
-black ; extra == "dev" Requires-Dist: bumpver ; extra == "dev" Requires-Dist:
-flit ; extra == "dev" Requires-Dist: pytest ; extra == "dev" Requires-Dist:
-sphinx ; extra == "dev" Requires-Dist: sphinx-rtd-theme ; extra == "dev"
-Project-URL: Homepage, https://stepmix.readthedocs.io/en/latest/ Provides-
-Extra: dev StepMix ============================== [PyPI_version] [![Build]
-(https://github.com/Labo-Lacourse/stepmix/actions/workflows/pytest.yaml/
+tqdm Requires-Dist: black ; extra == "dev" Requires-Dist: bumpver ; extra ==
+"dev" Requires-Dist: flit ; extra == "dev" Requires-Dist: pytest ; extra ==
+"dev" Requires-Dist: sphinx ; extra == "dev" Requires-Dist: sphinx-rtd-theme ;
+extra == "dev" Project-URL: Homepage, https://stepmix.readthedocs.io/en/latest/
+Provides-Extra: dev StepMix ============================== [PyPI_version] [!
+[Build](https://github.com/Labo-Lacourse/stepmix/actions/workflows/pytest.yaml/
 badge.svg)](https://github.com/Labo-Lacourse/stepmix/actions/workflows/
 pytest.yaml) [![Documentation Status](https://readthedocs.org/projects/stepmix/
 badge/?version=latest)](https://stepmix.readthedocs.io/en/latest/index.html)
 [Code_style:_black] [![Downloads](https://static.pepy.tech/badge/stepmix)]
 (https://pepy.tech/project/stepmix) [![Downloads](https://static.pepy.tech/
 badge/stepmix/month)](https://pepy.tech/project/stepmix) [![arXiv](https://
 img.shields.io/badge/arXiv-2304.03853-b31b1b.svg)](https://arxiv.org/abs/
```

