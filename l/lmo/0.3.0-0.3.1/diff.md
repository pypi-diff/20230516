# Comparing `tmp/lmo-0.3.0.tar.gz` & `tmp/lmo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.3.0.tar", max compression
+gzip compressed data, was "lmo-0.3.1.tar", max compression
```

## Comparing `lmo-0.3.0.tar` & `lmo-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.3.0/LICENSE
--rw-r--r--   0        0        0      754 2023-05-11 19:25:30.130399 lmo-0.3.0/README.md
--rw-r--r--   0        0        0      199 2023-05-02 23:21:30.443482 lmo-0.3.0/lmo/__init__.py
--rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.3.0/lmo/_meta.py
--rw-r--r--   0        0        0      415 2023-05-14 01:14:00.711613 lmo-0.3.0/lmo/_utils.py
--rw-r--r--   0        0        0     6933 2023-05-14 00:52:05.975764 lmo-0.3.0/lmo/multivariate.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.3.0/lmo/py.typed
--rw-r--r--   0        0        0     1099 2023-05-14 01:14:00.735614 lmo-0.3.0/lmo/stats.py
--rw-r--r--   0        0        0     1217 2023-05-14 00:52:26.476196 lmo-0.3.0/lmo/typing.py
--rw-r--r--   0        0        0     5727 2023-05-14 00:52:47.956648 lmo-0.3.0/lmo/univariate.py
--rw-r--r--   0        0        0     1527 2023-05-14 01:14:00.743614 lmo-0.3.0/lmo/weights.py
--rw-r--r--   0        0        0     1949 2023-05-14 01:18:45.937664 lmo-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lmo-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.3.1/LICENSE
+-rw-r--r--   0        0        0      772 2023-05-14 21:15:11.042568 lmo-0.3.1/README.md
+-rw-r--r--   0        0        0      199 2023-05-02 23:21:30.443482 lmo-0.3.1/lmo/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.3.1/lmo/_meta.py
+-rw-r--r--   0        0        0      415 2023-05-14 01:14:00.711613 lmo-0.3.1/lmo/_utils.py
+-rw-r--r--   0        0        0     7016 2023-05-16 21:16:49.054618 lmo-0.3.1/lmo/multivariate.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.3.1/lmo/py.typed
+-rw-r--r--   0        0        0     1099 2023-05-14 01:14:00.735614 lmo-0.3.1/lmo/stats.py
+-rw-r--r--   0        0        0     1230 2023-05-14 22:37:20.274592 lmo-0.3.1/lmo/typing.py
+-rw-r--r--   0        0        0     7402 2023-05-14 23:55:59.372417 lmo-0.3.1/lmo/univariate.py
+-rw-r--r--   0        0        0     1629 2023-05-14 22:28:48.803339 lmo-0.3.1/lmo/weights.py
+-rw-r--r--   0        0        0     1949 2023-05-16 21:19:57.918963 lmo-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 lmo-0.3.1/PKG-INFO
```

### Comparing `lmo-0.3.0/LICENSE` & `lmo-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.3.0/README.md` & `lmo-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-<img src="./docs/static/lmo.svg" alt="jorenham/lmo" width="128" align="right">
+<!--head-start-->
+
+<img src="https://jorenham.github.io/lmo/img/lmo.svg" alt="jorenham/lmo" width="128" align="right">
 
 # Lmo
 
-<!--badges-start-->
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jorenham/lmo/CI.yml?branch=master&style=flat-square)
 [![PyPI](https://img.shields.io/pypi/v/lmo?style=flat-square)](https://pypi.org/project/lmo/)
 [![versions](https://img.shields.io/pypi/pyversions/lmo?style=flat-square)](https://github.com/jorenham/lmo)
 [![license](https://img.shields.io/github/license/jorenham/lmo?style=flat-square)](https://github.com/jorenham/lmo/blob/master/LICENSE?)
-<!--badges-end-->
 
 
 Streamlined calculation of L-moments and TL-moments.
 
 ---
+<!--head-end-->
 
 [Documentation](https://jorenham.github.io/lmo/)
 
 ---
 
 *Examples coming soon*.
```

### Comparing `lmo-0.3.0/lmo/multivariate.py` & `lmo-0.3.1/lmo/multivariate.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,31 +104,35 @@
 # noinspection PyPep8Naming
 def tl_coratio(
     a: AnyMatrix,
     r: int,
     /,
     k: int = 2,
     trim: Trimming = 1,
+    *,
+    rowvar: bool = True,
     **kwargs: Any,
 ) -> npt.NDArray[np.float_]:
     """
     TL-comoment ratio matrix `L_r[i, j] / l_k[j]`.
 
     References:
         * Serfling, R. and Xiao, P., 2006. A Contribution to Multivariate
           L-Moments: L-Comoment Matrices.
 
     """
-    L_k = tl_comoment(a, r, trim, **kwargs)
+    L_k = tl_comoment(a, r, trim, rowvar=rowvar, **kwargs)
 
     if k == 0:
         return L_k
 
-    l_r = L_k.diagonal() if k == r else cast(
-        npt.NDArray[np.float_], tl_moment(a, r, trim, **kwargs)
+    axis = +rowvar
+    l_r = cast(
+        npt.NDArray[np.float_],
+        np.diag(L_k) if k == r else tl_moment(a, k, trim, axis=axis, **kwargs)
     )
 
     return L_k / l_r[:, np.newaxis]
 
 
 def tl_coloc(
     a: AnyMatrix,
```

### Comparing `lmo-0.3.0/lmo/stats.py` & `lmo-0.3.1/lmo/stats.py`

 * *Files identical despite different names*

### Comparing `lmo-0.3.0/lmo/typing.py` & `lmo-0.3.1/lmo/typing.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,14 +34,14 @@
 AnyMatrix: TypeAlias = AnyVector | Sequence[AnyVector]
 AnyTensor: TypeAlias = AnyMatrix | Sequence['AnyTensor']
 
 # complex numbers aren't relevant (and calling them scalars is far-fetched IMHO)
 ScalarOrArray: TypeAlias = _R | np.ndarray[Any, np.dtype[_R]]
 
 # for numpy.sort
-SortKind: TypeAlias = Literal['quicksort', 'heapsort', 'stable']
+SortKind: TypeAlias = Literal['quicksort', 'mergesort', 'heapsort', 'stable']
 
 # trim length
 _Trim0: TypeAlias = tuple[()]
 _Trim1: TypeAlias = tuple[int] | int
 _Trim2: TypeAlias = tuple[int, int]
 Trimming: TypeAlias = _Trim0 | _Trim1 | _Trim2
```

### Comparing `lmo-0.3.0/lmo/weights.py` & `lmo-0.3.1/lmo/weights.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,24 @@
 def tl_weights(n: int, r: int, /, trim: Trimming) -> npt.NDArray[np.float_]:
     """
     Linear sample weights for calculation of the r-th TL(s, t)-moment.
 
     Args:
         n: Sample size.
         r: L-moment order, e.g. 1 for location, and 2 for scale.
-        trim: Amount of samples to trim on both sides, or a tuple of the amount
-            to trim on the left and right sides. Default is 1.
+        trim:
+            Amount of samples to trim as either
+
+            - `(t1: int, t2: int)` for left and right trimming,
+            - `t: int`, or `(t: int)` as alias for `(t, t)`, or
+            - `()` as alias for `(0, 0)`.
 
     Returns:
-        w_j: A vector of size `n`, with linear weights for each of the
+        w_j:
+            A vector of size `n`, with linear weights for each of the
             (ordered) samples.
 
     """
     if r <= 0:
         raise ValueError(f'expected r > 0, got {r} <= 0')
 
     tl, tr = expand_trimming(trim)
```

### Comparing `lmo-0.3.0/pyproject.toml` & `lmo-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "lmo"
-version = "0.3.0"
+version = "0.3.1"
 description = "L-Moments for robust statistics."
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://jorenham.github.io/lmo/"
 repository = "https://github.com/jorenham/lmo/"
 classifiers = [
```

### Comparing `lmo-0.3.0/PKG-INFO` & `lmo-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.3.0
+Version: 0.3.1
 Summary: L-Moments for robust statistics.
 Home-page: https://jorenham.github.io/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -22,29 +22,30 @@
 Classifier: Typing :: Typed
 Requires-Dist: numpy (>=1.20,<2.0)
 Project-URL: Bug Tracker, https://github.com/jorenham/lmo/issues
 Project-URL: Documentation, https://jorenham.github.io/lmo/
 Project-URL: Repository, https://github.com/jorenham/lmo/
 Description-Content-Type: text/markdown
 
-<img src="./docs/static/lmo.svg" alt="jorenham/lmo" width="128" align="right">
+<!--head-start-->
+
+<img src="https://jorenham.github.io/lmo/img/lmo.svg" alt="jorenham/lmo" width="128" align="right">
 
 # Lmo
 
-<!--badges-start-->
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jorenham/lmo/CI.yml?branch=master&style=flat-square)
 [![PyPI](https://img.shields.io/pypi/v/lmo?style=flat-square)](https://pypi.org/project/lmo/)
 [![versions](https://img.shields.io/pypi/pyversions/lmo?style=flat-square)](https://github.com/jorenham/lmo)
 [![license](https://img.shields.io/github/license/jorenham/lmo?style=flat-square)](https://github.com/jorenham/lmo/blob/master/LICENSE?)
-<!--badges-end-->
 
 
 Streamlined calculation of L-moments and TL-moments.
 
 ---
+<!--head-end-->
 
 [Documentation](https://jorenham.github.io/lmo/)
 
 ---
 
 *Examples coming soon*.
```

