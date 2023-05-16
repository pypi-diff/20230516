# Comparing `tmp/spectrally_constrained_lvms-0.1.0.2.tar.gz` & `tmp/spectrally_constrained_lvms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrally_constrained_lvms-0.1.0.2.tar", max compression
+gzip compressed data, was "spectrally_constrained_lvms-0.1.1.tar", max compression
```

## Comparing `spectrally_constrained_lvms-0.1.0.2.tar` & `spectrally_constrained_lvms-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_constrained_lvms-0.1.0.2/LICENSE
--rw-r--r--   0        0        0     1616 2023-05-15 12:03:36.288103 spectrally_constrained_lvms-0.1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1289 2023-05-13 20:02:18.006810 spectrally_constrained_lvms-0.1.0.2/README.md
--rw-r--r--   0        0        0     1214 2023-05-15 11:46:26.325532 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/__init__.py
--rw-r--r--   0        0        0    16039 2023-05-13 15:58:08.511125 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/cost_functions.py
--rw-r--r--   0        0        0    21547 2023-05-13 15:56:12.827004 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/helper_methods.py
--rw-r--r--   0        0        0    15121 2023-05-13 15:42:49.428404 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/negen_approx.py
--rw-r--r--   0        0        0    16446 2023-05-13 15:41:10.612996 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/spectral_constraint.py
--rw-r--r--   0        0        0    31798 2023-05-15 11:57:51.356604 spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/spectrally_constrained_model.py
--rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.0.2/setup.py
--rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_constrained_lvms-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1777 2023-05-16 07:40:02.665593 spectrally_constrained_lvms-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1289 2023-05-13 20:02:18.006810 spectrally_constrained_lvms-0.1.1/README.md
+-rw-r--r--   0        0        0     1212 2023-05-16 07:40:02.681793 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/__init__.py
+-rw-r--r--   0        0        0    16084 2023-05-15 13:23:10.954638 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/cost_functions.py
+-rw-r--r--   0        0        0    21547 2023-05-13 15:56:12.827004 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/helper_methods.py
+-rw-r--r--   0        0        0    15121 2023-05-13 15:42:49.428404 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/negen_approx.py
+-rw-r--r--   0        0        0    16446 2023-05-13 15:41:10.612996 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/spectral_constraint.py
+-rw-r--r--   0        0        0    31979 2023-05-16 07:15:18.150362 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/spectrally_constrained_model.py
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.1/PKG-INFO
```

### Comparing `spectrally_constrained_lvms-0.1.0.2/LICENSE` & `spectrally_constrained_lvms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.0.2/pyproject.toml` & `spectrally_constrained_lvms-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "spectrally-constrained-LVMs"
-version = "0.1.0.2"
+version = "0.1.1"
 description = "An optimisation implementation of linear transforms with a spectral constraint."
 authors = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 maintainers = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://github.com/RyanBalshaw/scICA"
-repository = "https://github.com/RyanBalshaw/scICA"
-documentation = "https://github.com/RyanBalshaw/scICA"
-keywords = ["Linear transformation", "spectral constraint", "PCA", "ICA"]
+homepage = "https://github.com/RyanBalshaw/spectrally-constrained-LVMs"
+repository = "https://github.com/RyanBalshaw/spectrally-constrained-LVMs"
+documentation = "https://github.com/RyanBalshaw/spectrally-constrained-LVMs"
+keywords = ["Linear LVMs", "spectral constraint", "PCA", "ICA"]
 include = ["LICENSE"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation",
     "Topic :: Scientific/Engineering",
@@ -49,8 +49,10 @@
 sphinx-rtd-theme = ">=1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
-"Bug tracker" = "https://github.com/RyanBalshaw/scICA/issues"
+"Bug tracker" = "https://github.com/RyanBalshaw/spectrally-constrained-LVMs/issues"
+
+[tool.poetry_bumpversion.file."./spectrally_constrained_LVMs/__init__.py"] # Uses
```

### Comparing `spectrally_constrained_lvms-0.1.0.2/README.md` & `spectrally_constrained_lvms-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/__init__.py` & `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     quasi_Newton,
 )
 from .negen_approx import cube_object, exp_object, logcosh_object, quad_object
 from .spectral_constraint import spectral_objective
 from .spectrally_constrained_model import linear_model
 
 __author__ = "Ryan Balshaw"
-__version__ = "0.1.0.1"
+__version__ = "0.1.1"
 __email__ = "ryanbalshaw81@gmail.com"
 __description__ = (
     "Train linear LVMs with the addition "
     "of a spectral constraint with minimal effort."
 )
 # __uri__ = "http://spectrally-constrained-lvms.readthedocs.io/"
 __all__ = [
```

### Comparing `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/cost_functions.py` & `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/cost_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             f_b = self.cost(X, w0 - e_i, y)
 
             grad_check[i, 0] = (f_f - f_b) / (2 * step_size)
 
         grad_norm = np.linalg.norm(grad_current - grad_check)
 
         if self.verbose:
-            print(f"Finished! The gradient norm (row-wise) is: {np.round(grad_norm)}")
+            print(f"Finished! The gradient norm is: {np.round(grad_norm)}")
 
         return grad_current, grad_check, grad_norm
 
     def check_hessian(self, X, w, y, step_size):
         # Finite difference Hessian approximation (central difference)
 
         if self.verbose:
@@ -171,15 +171,15 @@
 
      Assumed format for methods: func(X, w, y) where X is an ndarray
       with shape (n_samples, n_features), w is an ndarray with shape (n_features, 1)
       and y is the linear transformation X @ w with shape (n_samples, 1).
 
     """
 
-    def __init__(self, use_hessian: bool, verbose=True):
+    def __init__(self, use_hessian: bool = True, verbose: bool =True):
         """
 
         Parameters
         ----------
         use_hessian : bool
             A flag to control whether you use the Hessian or not.
             This is useful in the solver, as you may wish to just
@@ -250,15 +250,15 @@
             return self._cost_hessian(X, w, y)
 
         else:
             return np.eye(w.shape[0])
 
 
 class sympy_cost(costClass):
-    def __init__(self, n_samples, n_features, use_hessian=False, verbose=True):
+    def __init__(self, n_samples: int, n_features: int, use_hessian: bool=False, verbose: bool=True):
         super().__init__(verbose)
         self.n_samples = n_samples
         self.n_features = n_features
         self.use_hessian = use_hessian
 
     def set_cost(self, cost_func):
         # overwrites the base method
@@ -372,15 +372,15 @@
             return self._cost_hessian(X, w, y)
 
         else:
             return np.eye(w.shape[0])
 
 
 class negentropy_cost(costClass):
-    def __init__(self, source_name: str, source_params: dict, verbose=True):
+    def __init__(self, source_name: str, source_params: dict, verbose: bool=True):
         super().__init__(verbose)
         self.source_name = source_name
         self.source_params = source_params  # dictionary of parameters
 
         # Initialise the source PDFs
         self.source_instance, self.source_expectation = initialise_sources(
             source_name, self.source_params
@@ -447,15 +447,15 @@
         # Calculate the Jacobian (Hessian)
         jacobian = -2 * (grad_outer + r * expectation)
 
         return jacobian
 
 
 class variance_cost(user_cost):
-    def __init__(self, use_hessian: bool, verbose=True):
+    def __init__(self, use_hessian: bool = True, verbose: bool =True):
         super().__init__(use_hessian, verbose)
 
         def loss(X, w, y):
             return -1 * np.mean((X @ w) ** 2, axis=0)
 
         def grad(X, w, y):
             return -2 * np.mean(y * X, axis=0, keepdims=True).T
```

### Comparing `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/helper_methods.py` & `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/helper_methods.py`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/negen_approx.py` & `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/negen_approx.py`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/spectral_constraint.py` & `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/spectral_constraint.py`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.0.2/spectrally_constrained_LVMs/spectrally_constrained_model.py` & `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/spectrally_constrained_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -883,15 +883,15 @@
         Y = np.dot(X_preprocess, self.W.T)
 
         self.excess_kurtosis_ = np.mean(Y**4, axis=0) - 3  # Excess kurtosis
 
         return self
 
     def transform(self, X):
-        return np.dot(self.preprocess_inst.preprocess_data(X), self.W.T)
+        return np.dot(self.processor_inst.preprocess_data(X), self.W.T)
 
     def inverse_transform(self, S):
         r, c = S.shape
 
         S_ = S.copy()
 
         # Transform back to the training feature space
@@ -917,9 +917,14 @@
             # val = 2/n * np.abs(
             #     np.fft.fft(ICA_model.Vh[i, :])[:n//2]
             # ) # Use this if you want to use PCA
             spectral_W[i, :] = val
 
         return spectral_W
 
-    def get_solver_results(self):
+    def get_model_parameters(self):
+        # TODO return dictionary of solution parameters.
         pass
+
+    def set_model_parameters(self):
+        # TODO input dictionary of solution parameters and set model.
+        pass
```

### Comparing `spectrally_constrained_lvms-0.1.0.2/PKG-INFO` & `spectrally_constrained_lvms-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: spectrally-constrained-lvms
-Version: 0.1.0.2
+Version: 0.1.1
 Summary: An optimisation implementation of linear transforms with a spectral constraint.
-Home-page: https://github.com/RyanBalshaw/scICA
+Home-page: https://github.com/RyanBalshaw/spectrally-constrained-LVMs
 License: MIT
-Keywords: Linear transformation,spectral constraint,PCA,ICA
+Keywords: Linear LVMs,spectral constraint,PCA,ICA
 Author: Ryan Balshaw
 Author-email: ryanbalshaw81@gmail.com
 Maintainer: Ryan Balshaw
 Maintainer-email: ryanbalshaw81@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -20,17 +20,17 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Requires-Dist: sympy (>=1.11.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Project-URL: Bug tracker, https://github.com/RyanBalshaw/scICA/issues
-Project-URL: Documentation, https://github.com/RyanBalshaw/scICA
-Project-URL: Repository, https://github.com/RyanBalshaw/scICA
+Project-URL: Bug tracker, https://github.com/RyanBalshaw/spectrally-constrained-LVMs/issues
+Project-URL: Documentation, https://github.com/RyanBalshaw/spectrally-constrained-LVMs
+Project-URL: Repository, https://github.com/RyanBalshaw/spectrally-constrained-LVMs
 Description-Content-Type: text/markdown
 
 # Spectrally constrained LVMs
 
 ![GitHub](https://img.shields.io/github/license/RyanBalshaw/spectrally-constrained-LVMs)
 ![GitHub issues](https://img.shields.io/github/issues-raw/RyanBalshaw/spectrally-constrained-LVMs)
 ![PyPI](https://img.shields.io/pypi/v/spectrally-constrained-lvms)
```

