# Comparing `tmp/coola-0.0.6.tar.gz` & `tmp/coola-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coola-0.0.6.tar", max compression
+gzip compressed data, was "coola-0.0.7.tar", max compression
```

## Comparing `coola-0.0.6.tar` & `coola-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1501 2023-04-15 03:00:55.142524 coola-0.0.6/LICENSE
--rw-r--r--   0        0        0     4491 2023-04-15 03:00:55.142524 coola-0.0.6/README.md
--rw-r--r--   0        0        0     4113 2023-04-15 03:00:55.146524 coola-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      681 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/__init__.py
--rw-r--r--   0        0        0    18460 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/allclose.py
--rw-r--r--   0        0        0    13171 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/equality.py
--rw-r--r--   0        0        0     2444 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/format.py
--rw-r--r--   0        0        0     1195 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/import_utils.py
--rw-r--r--   0        0        0     4260 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/ndarray.py
--rw-r--r--   0        0        0     7521 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/pytorch.py
--rw-r--r--   0        0        0      297 2023-04-15 03:00:55.146524 coola-0.0.6/src/coola/testing.py
--rw-r--r--   0        0        0     5791 1970-01-01 00:00:00.000000 coola-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-16 02:38:26.151940 coola-0.0.7/LICENSE
+-rw-r--r--   0        0        0     5049 2023-05-16 02:38:26.151940 coola-0.0.7/README.md
+-rw-r--r--   0        0        0     4111 2023-05-16 02:38:26.151940 coola-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      682 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/__init__.py
+-rw-r--r--   0        0        0    18466 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/allclose.py
+-rw-r--r--   0        0        0    13177 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/equality.py
+-rw-r--r--   0        0        0     4261 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/ndarray.py
+-rw-r--r--   0        0        0     7522 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/pytorch.py
+-rw-r--r--   0        0        0      297 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/testing.py
+-rw-r--r--   0        0        0        0 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/utils/__init__.py
+-rw-r--r--   0        0        0     2456 2023-05-16 02:38:26.151940 coola-0.0.7/src/coola/utils/format.py
+-rw-r--r--   0        0        0     1195 2023-05-16 02:38:26.155939 coola-0.0.7/src/coola/utils/imports.py
+-rw-r--r--   0        0        0     6349 1970-01-01 00:00:00.000000 coola-0.0.7/PKG-INFO
```

### Comparing `coola-0.0.6/LICENSE` & `coola-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `coola-0.0.6/README.md` & `coola-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 # coola
 
 <p align="center">
     <a href="https://github.com/durandtibo/coola/actions">
         <img alt="CI" src="https://github.com/durandtibo/coola/workflows/CI/badge.svg?event=push&branch=main">
     </a>
+    <a href="https://durandtibo.github.io/coola/">
+        <img alt="CI" src="https://github.com/durandtibo/coola/workflows/Documentation/badge.svg?event=push&branch=main">
+    </a>
+    <a href="https://codecov.io/gh/durandtibo/coola">
+        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/coola/branch/main/graph/badge.svg">
+    </a>
+    <a href="https://codeclimate.com/github/durandtibo/coola/maintainability">
+        <img src="https://api.codeclimate.com/v1/badges/83ebb50e6c6f67b0570d/maintainability" />
+    </a>
+    <a href="https://codeclimate.com/github/durandtibo/coola/test_coverage">
+        <img src="https://api.codeclimate.com/v1/badges/83ebb50e6c6f67b0570d/test_coverage" />
+    </a>
+    <br/>
     <a href="https://pypi.org/project/coola/">
         <img alt="PYPI version" src="https://img.shields.io/pypi/v/coola">
     </a>
     <a href="https://pypi.org/project/coola/">
         <img alt="Python" src="https://img.shields.io/pypi/pyversions/coola.svg">
     </a>
     <a href="https://opensource.org/licenses/BSD-3-Clause">
         <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/coola">
     </a>
-    <a href="https://codecov.io/gh/durandtibo/coola">
-        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/coola/branch/main/graph/badge.svg">
-    </a>
     <a href="https://github.com/psf/black">
         <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
     </a>
     <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
         <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
     </a>
     <br/>
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
 # coola
-[CI] [PYPI_version] [Python] [BSD-3-Clause] [Codecov] [Code_style:_black] [Doc
-                                style:_google]
+          [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
+ 83ebb50e6c6f67b0570d/maintainability] [https://api.codeclimate.com/v1/badges/
+                     83ebb50e6c6f67b0570d/test_coverage]
+[PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
 ## Overview `coola` is a light Python library that provides simple functions to
 check in a single line if two complex/nested objects are equal or not. `coola`
 was initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/
 docs/stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
 reference/generated/numpy.ndarray.html), but it is possible to extend it to
 [support other data structures](https://durandtibo.github.io/coola/
```

### Comparing `coola-0.0.6/pyproject.toml` & `coola-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coola"
-version = "0.0.6"
+version = "0.0.7"
 description = "A light library to check if two complex/nested objects are equal or not"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/coola"
 repository = "https://github.com/durandtibo/coola"
 keywords = ["equality", "complex/nested objects"]
 license = "BSD-3-Clause"
@@ -90,16 +90,14 @@
 
 [tool.docformatter]
 recursive = true
 wrap-summaries = 72
 wrap-descriptions = 72
 syntax = "google"
 
-
-
 [tool.ruff]
 select = [
     "A",   # builtins
     "ANN", # annotations
     "B",   # bugbear
     "BLE", # blind-except
     "E",   # pycodestyle (Error)
```

### Comparing `coola-0.0.6/src/coola/__init__.py` & `coola-0.0.7/src/coola/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 )
 from coola.equality import (
     BaseEqualityOperator,
     BaseEqualityTester,
     EqualityTester,
     objects_are_equal,
 )
-from coola.import_utils import is_numpy_available, is_torch_available
+from coola.utils.imports import is_numpy_available, is_torch_available
 
 if is_numpy_available():
     from coola import ndarray  # noqa: F401
 
 if is_torch_available():
     from coola import pytorch  # noqa: F401
```

### Comparing `coola-0.0.6/src/coola/allclose.py` & `coola-0.0.7/src/coola/allclose.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import logging
 import math
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
 from typing import Any, Generic, Optional, TypeVar, Union
 
-from coola.format import str_dict, str_indent
+from coola.utils.format import str_dict, str_indent
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 class BaseAllCloseTester(ABC):
```

### Comparing `coola-0.0.6/src/coola/equality.py` & `coola-0.0.7/src/coola/equality.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
 from typing import Any, Generic, Optional, TypeVar
 
-from coola.format import str_dict, str_indent
+from coola.utils.format import str_dict, str_indent
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 class BaseEqualityTester(ABC):
```

### Comparing `coola-0.0.6/src/coola/format.py` & `coola-0.0.7/src/coola/utils/format.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Returns:
         str: The string representation.
 
         Example usage:
 
     .. code-block:: python
 
-        >>> from coola.format import str_dict
+        >>> from coola.utils.format import str_dict
         >>> str_dict({"my_key": "my_value"})
         'my_key : my_value'
         >>> str_dict({"key1": "value1", "key2": "value2"})
         'key1 : value1\nkey2 : value2'
     """
     if indent < 0:
         raise ValueError(f"The indent has to be greater or equal to 0 (received: {indent})")
@@ -56,15 +56,15 @@
     Returns:
         str: The indented string.
 
     Example usage:
 
     .. code-block:: python
 
-        >>> from coola.format import str_indent
+        >>> from coola.utils.format import str_indent
         >>> print(f"\t{str_indent('string1\nstring2', 4)}")
             string1
             string2
     """
     formatted_str = str(original).split("\n")
     if len(formatted_str) == 1:  # single line
         return formatted_str[0]
```

### Comparing `coola-0.0.6/src/coola/import_utils.py` & `coola-0.0.7/src/coola/utils/imports.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.6/src/coola/ndarray.py` & `coola-0.0.7/src/coola/ndarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = ["NDArrayAllCloseOperator", "NDArrayEqualityOperator"]
 
 import logging
 from typing import Any
 
 from coola.allclose import AllCloseTester, BaseAllCloseOperator, BaseAllCloseTester
 from coola.equality import BaseEqualityOperator, BaseEqualityTester, EqualityTester
-from coola.import_utils import check_numpy, is_numpy_available
+from coola.utils.imports import check_numpy, is_numpy_available
 
 if is_numpy_available():
     from numpy import allclose, array_equal, ndarray
 else:
     ndarray, array_equal, allclose = None, None, None  # pragma: no cover
 
 logger = logging.getLogger(__name__)
```

### Comparing `coola-0.0.6/src/coola/pytorch.py` & `coola-0.0.7/src/coola/pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 import logging
 from typing import Any
 
 from coola.allclose import AllCloseTester, BaseAllCloseOperator, BaseAllCloseTester
 from coola.equality import BaseEqualityOperator, BaseEqualityTester, EqualityTester
-from coola.import_utils import check_torch, is_torch_available
+from coola.utils.imports import check_torch, is_torch_available
 
 if is_torch_available():
     from torch import Tensor, is_tensor
     from torch.nn.utils.rnn import PackedSequence
 else:
     PackedSequence, Tensor, is_tensor = None, None, None  # pragma: no cover
```

### Comparing `coola-0.0.6/PKG-INFO` & `coola-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coola
-Version: 0.0.6
+Version: 0.0.7
 Summary: A light library to check if two complex/nested objects are equal or not
 Home-page: https://github.com/durandtibo/coola
 License: BSD-3-Clause
 Keywords: equality,complex/nested objects
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -31,26 +31,36 @@
 
 # coola
 
 <p align="center">
     <a href="https://github.com/durandtibo/coola/actions">
         <img alt="CI" src="https://github.com/durandtibo/coola/workflows/CI/badge.svg?event=push&branch=main">
     </a>
+    <a href="https://durandtibo.github.io/coola/">
+        <img alt="CI" src="https://github.com/durandtibo/coola/workflows/Documentation/badge.svg?event=push&branch=main">
+    </a>
+    <a href="https://codecov.io/gh/durandtibo/coola">
+        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/coola/branch/main/graph/badge.svg">
+    </a>
+    <a href="https://codeclimate.com/github/durandtibo/coola/maintainability">
+        <img src="https://api.codeclimate.com/v1/badges/83ebb50e6c6f67b0570d/maintainability" />
+    </a>
+    <a href="https://codeclimate.com/github/durandtibo/coola/test_coverage">
+        <img src="https://api.codeclimate.com/v1/badges/83ebb50e6c6f67b0570d/test_coverage" />
+    </a>
+    <br/>
     <a href="https://pypi.org/project/coola/">
         <img alt="PYPI version" src="https://img.shields.io/pypi/v/coola">
     </a>
     <a href="https://pypi.org/project/coola/">
         <img alt="Python" src="https://img.shields.io/pypi/pyversions/coola.svg">
     </a>
     <a href="https://opensource.org/licenses/BSD-3-Clause">
         <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/coola">
     </a>
-    <a href="https://codecov.io/gh/durandtibo/coola">
-        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/coola/branch/main/graph/badge.svg">
-    </a>
     <a href="https://github.com/psf/black">
         <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
     </a>
     <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
         <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
     </a>
     <br/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coola Version: 0.0.6 Summary: A light library to
+Metadata-Version: 2.1 Name: coola Version: 0.0.7 Summary: A light library to
 check if two complex/nested objects are equal or not Home-page: https://
 github.com/durandtibo/coola License: BSD-3-Clause Keywords: equality,complex/
 nested objects Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
@@ -12,16 +12,18 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Software Development ::
 Libraries Provides-Extra: all Requires-Dist: numpy (>=1.20,<2.0) ; extra ==
 "all" Requires-Dist: torch (>=1.10,<3.0) ; extra == "all" Project-URL:
 Repository, https://github.com/durandtibo/coola Description-Content-Type: text/
 markdown # coola
-[CI] [PYPI_version] [Python] [BSD-3-Clause] [Codecov] [Code_style:_black] [Doc
-                                style:_google]
+          [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
+ 83ebb50e6c6f67b0570d/maintainability] [https://api.codeclimate.com/v1/badges/
+                     83ebb50e6c6f67b0570d/test_coverage]
+[PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
 ## Overview `coola` is a light Python library that provides simple functions to
 check in a single line if two complex/nested objects are equal or not. `coola`
 was initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/
 docs/stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
 reference/generated/numpy.ndarray.html), but it is possible to extend it to
 [support other data structures](https://durandtibo.github.io/coola/
```

